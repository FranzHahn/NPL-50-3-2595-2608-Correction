# NPL-50-3-Correction

This project contains code to reproduce the results published in [Critical analysis on the reproducibility of visual quality assessment using deep features](https://arxiv.org/abs/2009.05369). 

`main_no_ft.m` is the entry point for the reproduction of results without fine-tuning, while `main_ft.m` handles the case with fine-tuning. The code requires a `videos/` folder with the KoNViD-1k videos in the root directory, which can be downloaded as a tarball [here](https://datasets.vqa.mmsp-kn.de/plosone/nepl/videos.tar.gz).

The `results/` subfolder contains MATLAB binaries containing the results of both procedures. Run `results.m` to reproduce the values in rows 8 and 12-15 in Table 2 in the paper, also reproduced below.

By running the code several derivative datastructures are created, which have been pre-computed by us and provided here:

- `frames/`: all the individual video frames are extracted here. [Download](https://datasets.vqa.mmsp-kn.de/plosone/nepl/frames.tar.gz)
- `networks/`: fine-tuned networks are saved here. [Download](https://datasets.vqa.mmsp-kn.de/plosone/nepl/networks.tar.gz)
- `features/`: features for all videos extracted from the networks (with and without fine-tuning) are stored here. [Download](https://datasets.vqa.mmsp-kn.de/plosone/nepl/features.tar.gz)

![Results Table](https://github.com/FranzHahn/NPL-50-3-2595-2608-Correction/raw/master/figures/resulttable.png "Results Table")