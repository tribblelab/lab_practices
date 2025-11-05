# Software Guide

This document provides suggestions (not requirements) for software that facilitates the research we do. Please use the ``issues `` feature on GitHub to suggest changes to this document.

Guiding principles: 

- Software should be effective and make the work easier, not harder
- Software should be as lightweight as possible (no unnecessary features or bloat)
- Software should be open source and free whenever possible
- Software should facilitate collaboration, sharing your work, and documenting your process 

## Google vs. Microsoft 

In general, the Tribble lab prefers to use Google-based tools such as Google Calendar, GMail, etc. for our work. Any lab members with strong preferences for Microsoft will not be forced to convert :) 

## Citation managers

Citation managers help you keep track of papers or other sources. They often allow you to link a PDF of a paper with your own notes and export the citation for the paper in a variety of formats. PI Carrie is ashamed to admit that I use a plain text document instead of actual software (see the discussion about Latex, below), but my sleuthing had deduced that [Zotero](https://guides.lib.uw.edu/research/zotero) is a popular choice.

For more on citation managers, reach out the [UW Library](https://lib.uw.edu/about/contact/). Librarians are incredible, underutilized resources. Also check out a recorded workshop on citation managers available [here](http://www.lib.washington.edu/commons/services/workshops/citations?_gl=1*qpbden*_ga*NjEyODUxMjg2LjE3MjIxOTI0NTE.*_ga_63X2ZQHK8P*MTcyODE0MjU3Mi42LjEuMTcyODE0MzE0Ny4wLjAuMA..). 

## Text processing 

### For typesetting (writing papers, etc.) 

Microsoft Word (available through UW [here](https://itconnect.uw.edu/uware/microsoft-office-for-desktop/)) is a classic option for writing anything from your grocery list to a scientific article. However, cloud-based tools like [Google Docs](docs.google.com) make collaborative writing easier. 

``LaTeX`` is a software system for typesetting documents and is an alternative to programs like Word or Google Docs. ``LaTeX`` works similarly to a coding language, where users specify all aspects of formating (such as italics, text size, figure placement, citations, mathematical equations) with code. The feel of writing in ``Latex`` can take a bit of getting used to (similar to using HTML or Markdown), but it hugely improves the user's ability to control formatting in the document and is almost necessary for writing papers with mathematical notation. 

``LaTeX`` has a steep learning curve but is the preferred text processing software for writing papers in the lab. There is a web-based interface for ``LaTeX`` called [Overleaf](https://www.overleaf.com/) that greatly improves collabration on ``LaTeX`` documents. Overleaf also provides a nice introductory [tutorial](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes) for new users. Overleaf is available for free, but UW also provides access to a [Professional Upgrade](https://admin.artsci.washington.edu/computing/overleaf-latex-editor-professional-upgrade). I have made an article template on Overleaf, available [here](https://www.overleaf.com/read/nyfwbfyjqrxb#f681a1). 

Citations are also formatted for ``LaTeX`` documents using ``BibTex``. Tutorial [here](https://www.economics.utoronto.ca/osborne/latex/BIBTEX.HTM).   

### For visualizing and editing plain text files (code, etc.)

[Sublime Text](https://www.sublimetext.com/) is a good and simple plain text editor. [VSCode](https://code.visualstudio.com/) is a more feature-rich integrated development environment. While both are great options, VSCode offers more features and won't pop open a window every few hours asking you to pay for an upgrade. 

## Data storage 

Data should be stored on the lab network-attached storage (NAS) device. Data used in publications should be made available on Zenodo and linked to the lab's [Zenodo organization](https://zenodo.org/communities/tribblelab/). Unprocessed sequence data should be made available on NCBI's [Sequence Read Archive](https://www.ncbi.nlm.nih.gov/sra) or [GenBank](https://www.ncbi.nlm.nih.gov/genbank/) as appropriate, and processed data should be included in Zenodo. 

## Computer backups 

It is required that all lab members working on lab-related research on their personal computers have a cloud and/or physical backup system for their computer. I use [Backblaze](https://www.backblaze.com/) and have been happy with it. iCloud or other similar systems are also acceptable. The main point is that **you should always be able to recover all files on your computer with a 24 hr buffer if your computer is destroyed, lost, or stolen**. If you do not have access to a back-up system, talk to me [Carrie] and I will provide one. 

## Version control 

The lab uses GitHub (where you are now) to faciliate version control and collaborative work when writing code. A good introduction to GitHub and version control with ``git`` can be found [here](https://swcarpentry.github.io/git-novice/). Are you a trailblazer and desperately want to use Bitbucket, etc.? Let's talk. 

Note: when creating repos within the lab GitHub organization, to ``clone`` & then edit your repository on your computer or to a cluster like HYAK, you will probably need SSH key log-in credentials (not using the HTTPS URL method). Follow the instructions [here](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) to generate an SSH key on either your computer or the cluster. Then follow the instructions [here](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) to add your newly generated SSH key to your GitHub account. Once you've done so, you can ``git clone`` your repository like so: ``git clone git@github.com:tribblelab/lab_practices.git``. (That last bit of that command will be different for each repostitory. You can find yours if you're in your repository home page, then click the green "Code" button, then click the SSH tab under "Clone").

## Communication tools

The lab uses Slack to communicate day-to-day and as a group. Emails are best for larger asks, such as looking over a paper draft, letters of recommendation, etc. Slack is great for "who left Sleepless in Seattle playing on the lab computer?" or "does anyone have a copy of the Flora of the Pacific Northwest I can borrow to identify this cool plant I saw last weekend?" or "Help! I keep getting this error in R and I can't figure out why." 

