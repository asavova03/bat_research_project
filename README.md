# Auditory Kernels of Bat Vocalizations

Code repository for the bachelor's thesis "Testing the Efficient Coding Hypothesis beyond Humans: the Auditory Kernels of Bat Vocalizations" ([full paper](https://resolver.tudelft.nl/uuid:f7d76b24-ee79-46ea-a85d-78fcbdfbafff)).

## Overview

This repository contains code and trained kernels for learning sparse auditory representations of bat vocalizations using matching pursuit. The project tests the efficient coding hypothesis by training and analyzing auditory kernels on echolocation vocalizations of the *Rhinolophus affinis* species, sourced from the ChiroVox bat vocalization dataset, using different initialization parameters and frequency ranges.

## Repository Contents

### Notebooks
- `download.ipynb` - Script to download the Chirovox dataset
- `preprocess.ipynb` - Denoising and bat call segmentation
- `analysis.ipynb` - Preliminary analysis and visualization of learned kernels
- `results.ipynb` - Results comparison and plotting

### Utilities
- `mp_utils.py` - Matching pursuit utility functions

### Trained Kernels
Pre-trained auditory kernels in `.jld2` format with varying parameters:

**All frequencies:**
- `kernels_all_100_10000.jld2` - 100 frames, 10000 iterations
- `kernels_all_400_10000.jld2` - 400 frames, 10000 iterations

**High frequency (peak > 25 kHz):**
- `kernels_high_100_10000.jld2` - 100 frames, 10000 iterations
- `kernels_high_400_10000.jld2` - 400 frames, 10000 iterations

**Low frequency (peak < 25 kHz):**
- `kernels_low_100_5000.jld2` - 100 frames, 5000 iterations
- `kernels_low_400_5000.jld2` - 400 frames, 5000 iterations

## Citation

If you use this code, please cite the thesis:
```
Testing the Efficient Coding Hypothesis beyond Humans: the Auditory Kernels of Bat Vocalizations
TU Delft Repository, 2024
https://resolver.tudelft.nl/uuid:f7d76b24-ee79-46ea-a85d-78fcbdfbafff
```
