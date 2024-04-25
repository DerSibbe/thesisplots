# thesisplots

This repository contains the full set of evaluation plots for my bachelor's thesis "Recent Advances in Single-Channel Speech Separation of Same-Gender Speaker Mixtures".

The structure and filenames of this repository are explained below.

### Directories:

The three directories correspond to the three sections of "Evaluation 2: Separation of mixtures by speakers’ fundamental frequencies":

- eval_f0_avg: contains all plots showing the results on each individual test mixture, organized by the speakers' average speaking fundamental frequency.  
- eval_f0_diff: contains all plots showing the results on each individual test mixture, organized by the difference between the speakers' average speaking fundamental frequencies.  
- eval_f0_std: contains all plots showing the results on each individual test mixture, organized by the standard deviation of the speakers' speaking fundamental frequency.  

Within each, there's one subdirectory per evaluated separation model:

- chimerapp8kHz: contains plots for the evaluation of Chimera++
- convtasnet8kHz: contains plots for the evaluation of Conv-TasNet
- diffsep: contains plots for the evaluation of DiffSep
- sepformer: contains plots for the evaluation of SepFormer
- mossformer: contains plots for the evaluation of MossFormer

### Filenames:

- pesq: plot shows PESQ results for each individual file
- sisdr: plot shows SI-SDR results for each individual file
- sisnr: plot shows SI-SNR results for each individual file
- stoi: plot shows STOI results for each individual file

For eval_f0_avg and eval_f0_std:

- total: plot shows results for all test mixtures
- mf: plot shows results only for test mixtures with one male and one female speaker 
- mm: plot shows results only for test mixtures with two male speakers
- ff: plot shows results only for test mixtures with two female speakers

### Example:

eval_f0_avg/convtasnet8kHz/convtasnet8kHz_mf_sisnr.png shows the SI-SNR results of Conv-TasNet on all test mixtures with one male and one female speaker, organized by the average speaking fundamental frequencies of both speakers.
