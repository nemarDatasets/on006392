[![DOI](https://img.shields.io/badge/DOI-10.82901%2Fnemar.on006392-blue)](https://doi.org/10.82901/nemar.on006392)

# BIDS example with HED-SCORE schema library annotations

The HED schema library for the Standardized Computer-based Organized Reporting of EEG (SCORE) can be used to add annotations for BIDS datasets. The annotations are machine readable and validated with the BIDS and HED validators. 

This example is related to the following preprint:
Dora Hermes, Tal Pal Attia, Sándor Beniczky, Jorge Bosch-Bayard, Arnaud Delorme, Brian Nils Lundstrom, Christine Rogers, Stefan Rampp, Seyed Yahya Shirazi, Dung Truong, Pedro Valdes-Sosa, Greg Worrell, Scott Makeig, Kay Robbins. Hierarchical Event Descriptor library schema for EEG data annotation. arXiv preprint arXiv:2310.15173. 2024 Oct 27.

# General information
This BIDS example dataset includes iEEG data from one subject that were measured during clinical photic stimulation. Intracranial EEG data were collected at Mayo Clinic Rochester, MN under IRB#: 15-006530.  

# Events
The events are annotated according to the HED-SCORE schema library. Data are annotated by adding a column for annotations in the _events.tsv. The levels and annotations in this column are defined in the _events.json sidecar as HED tags. 

# More information
HED: https://www.hedtags.org/
HED schema library for SCORE: https://github.com/hed-standard/hed-schema-library 

# Contact
Dora Hermes: hermes.dora@mayo.edu

## Channels table generated from the data header (18 Oct 2026)

1 recording(s) had no channels.tsv, which BIDS requires for iEEG (bids-validator and `mne_bids` could not attach channel types or units). `sub-ieegModulator_ses-ieeg01_task-photicstim_run-01_channels.tsv` now lists the 194 channels of the MEF 3 channel directories (`<name>.timd`, ordered by acquisition_channel_number) and their `.tmet` metadata (sampling frequency, units): names and sampling frequency from the header, units from the header, type from the name (ECG/EMG/EOG/trigger) or, for contacts listed in electrodes.tsv, the iEEG type of the *_ieeg.json channel counts, scalp 10-20 labels not in electrodes.tsv EEG, otherwise MISC (types: ECG 1, EEG 21, SEEG 172); status n/a (no former status exists).

Note: `sub-ieegModulator_ses-ieeg01_task-photicstim_run-01_ieeg.json` channel counts set to the generated channels.tsv: SEEGChannelCount 166 -> 172.
