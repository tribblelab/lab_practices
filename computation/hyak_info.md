# Info for shared computational resources on HYAK

## Software install

### CAPTUS

[CAPTUS](https://github.com/edgardomortiz/captus) is a pipeline for assembling high-throughput sequencing reads.

to be done ONCE:
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

then to have your *own* conda env look in the right place (aka add it to its path):
1. `nano ~/.condarc`
2. add lines
```
pkgs_dirs:
  - /gscratch/tribblelab/conda/conda_pkgs
```

hereafter, to load in the `captus` conda env *interactively*:
```{bash}
salloc --partition=cpu-g2 --cpus-per-task=1 --mem=10G --time=2:00:00
module load conda
conda activate /gscratch/tribblelab/conda/captus
```

## Storage on HYAK

### Checking storage status

Run command `hyakstorage` to get the status of both individual user + `gscratch/tribblelab` disk/file usage.

### Requesting additional storage

1. Disk storage: submit request through [form here](https://uwconnect.uw.edu/it?id=sc_cat_item&sys_id=784e3d6c873e9a106f1997dd3fbb35b5)
> Supplemental storage on Hyak is available for Hyak group account owners at a monthly rate of $10.00 per TB per month (with a limit of 1 million inodes per TB).
2. File storage: email help@uw.edu with subject line "Hyak storage"
