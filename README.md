Singapore "EFFO2" Dataset (`singapore-effo2-bids`)

## Overview

**NB**: This dataset is one of three datasets (`singapore-alfie-bids`, `singapore-cheevul-bids`, and `singapore-effo2-bids`) that make up the Singapore sample.

This dataset contains MRI data from a sleep manipulation study conducted at the National University of Singapore (Singapore). It is part of the ENIGMA-Sleep Working Group collection used to study the effects of sleep loss on glymphatic MRI indices. The data are organized according to the Brain Imaging Data Structure (BIDS) and managed with DataLad (git-annex).

## Sample

| Item | Value |
|---|---|
| Site | Singapore |
| Affiliation | National University of Singapore |
| Country | Singapore |
| Participants (N) | 66 |
| Age, mean (SD), years | 22.0 (2.3) |
| Male (%) | 50.0 |

## Sleep protocol

- **BL**: baseline, habitual
- **SD**: total sleep deprivation, 24h

## Imaging data

### T1-weighted (`anat/`)

| Parameter | Value |
|---|---|
| Scanner | Siemens TrioTim |
| Sequence | MPRAGE |
| TR (ms) | 2000 |
| TE (ms) | 2.98 |
| TI (ms) | 900 |
| Flip angle (°) | 9 |

## Data organization

- `sub-<ID>/ses-<label>/`: raw BIDS data (`anat/`)
- `participants.tsv`: participant-level information
- `sub-<ID>/sub-<ID>_sessions.tsv`: session-level information (condition, visit, date, time)
- `derivatives/`: processed outputs, if present

File contents are tracked with git-annex. After cloning, retrieve data with `datalad get <path>`.

## Original publication

Yeo, B. T. T., Tandi, J., & Chee, M. W. L. (2015). Functional connectivity during rested wakefulness predicts vulnerability to sleep deprivation. *NeuroImage*, 111, 147–158. [https://doi.org/10.1016/j.neuroimage.2015.02.018](https://doi.org/10.1016/j.neuroimage.2015.02.018)

## Contact

- Jorik D. Elberse: [j.elberse@fz-juelich.de](mailto:j.elberse@fz-juelich.de)
- Masoud Tahmasian: [m.tahmasian@fz-juelich.de](mailto:m.tahmasian@fz-juelich.de)
