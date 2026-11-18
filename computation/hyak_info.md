# Info for shared computational resources on HYAK

## Shared group software install / usage

### CAPTUS

[CAPTUS](https://github.com/edgardomortiz/captus) is a pipeline for assembling high-throughput sequencing reads.

#### install 
to be done ONCE: (already done by lauren 2026-08-18)
```{bash}
salloc --partition=cpu-g2 --cpus-per-task=1 --mem=10G --time=2:00:00
module load conda
conda create --prefix /gscratch/tribblelab/conda/captus \
  -c bioconda -c conda-forge \
  captus bbmap=39.80 salmon=1.10.3 mafft=7.526

chmod -R g+rX /gscratch/tribblelab/conda/captus

conda env export --prefix /gscratch/tribblelab/conda/captus --no-builds \
  > /gscratch/tribblelab/conda/captus_environment.yml
```
here, I call an interactive node, load the `conda` module available on HYAK, then create the `captus` conda env.

#### usage

then to have your *own* conda env look in the right place (aka add it to its path):
1. `nano ~/.condarc`
2. add lines
```
pkgs_dirs:
  - /gscratch/tribblelab/conda
```

hereafter, to load in the `captus` conda env *interactively*:
```{bash}
salloc --partition=cpu-g2 --cpus-per-task=1 --mem=10G --time=2:00:00
module load conda
conda activate /gscratch/tribblelab/conda/captus
```

or, in a script submitted via slurm, just add these lines:
```{bash}
module load conda
conda activate /gscratch/tribblelab/conda/captus
```

### GetOrganelle

[GetOrganelle](https://github.com/kinggerm/getorganelle) is a pipeline for assembling organellar genomes (plastomes).

#### install 

to be done ONCE: (already done by lauren 2026-11-18)
```{bash}
# Create the shared env. conda-forge goes first so libsqlite etc. resolve.
conda create --prefix /gscratch/tribblelab/conda/getorganelle \
  --override-channels --strict-channel-priority \
  -c conda-forge -c bioconda \
  getorganelle

# Download the seed/label databases once, into a shared location (see note below)
mkdir -p /gscratch/tribblelab/conda/getorganelle_db
conda activate /gscratch/tribblelab/conda/getorganelle
export GETORG_PATH=/gscratch/tribblelab/conda/getorganelle_db
get_organelle_config.py --add embplant_pt,embplant_mt,embplant_nr

# Make everything readable and executable by the group
chmod -R g+rX /gscratch/tribblelab/conda/getorganelle \
              /gscratch/tribblelab/conda/getorganelle_db

# Export a reproducible spec
conda env export --prefix /gscratch/tribblelab/conda/getorganelle --no-builds \
  > /gscratch/tribblelab/conda/getorganelle_environment.yml
```

#### usage

if you haven't set up CAPTUS for your account, follow the same instructions as above to add
`/gscratch/tribblelab/conda` to your $PATH:

1. `nano ~/.condarc`
2. add lines
```
pkgs_dirs:
  - /gscratch/tribblelab/conda
```

hereafter, to load in the `getorganelle` conda env *interactively*:
```{bash}
salloc --partition=cpu-g2 --cpus-per-task=1 --mem=10G --time=2:00:00
module load conda
conda activate /gscratch/tribblelab/conda/getorganelle
```

or, in a script submitted via slurm, just add these lines:
```{bash}
module load conda
conda activate /gscratch/tribblelab/conda/getorganelle
```

## Storage on HYAK

### Checking storage status

Run command `hyakstorage` to get the status of both individual user + `gscratch/tribblelab` disk/file usage.

### Requesting additional storage

1. Disk storage: submit request through [form here](https://uwconnect.uw.edu/it?id=sc_cat_item&sys_id=784e3d6c873e9a106f1997dd3fbb35b5)
> Supplemental storage on Hyak is available for Hyak group account owners at a monthly rate of $10.00 per TB per month (with a limit of 1 million inodes per TB).
2. File storage: email help@uw.edu with subject line "Hyak storage"
