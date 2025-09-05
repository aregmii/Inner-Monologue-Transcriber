# Decoding Imagined Speech: A Novel Transformer Architecture for EEG-to-Text

This project aims to set a new state-of-the-art for decoding continuous, sentence-level imagined speech from non-invasive EEG.

### The Challenge

Recent research (Bao et al., 2025) on the Chisco-2.0 dataset—the same one used in this project—suggests that achieving high-performance decoding with current methods would require an estimated 15.7 years of data from a single user. This highlights a massive data-efficiency gap in the field.

### Approach

This project tackles that challenge head-on by developing a novel sequence-to-sequence Transformer model that leverages an enriched feature representation combining spectral, spatial, and phase information from the EEG signal.

The goal is to be the first to establish a credible Word Error Rate (WER) benchmark for sentence-level transcription on this dataset, demonstrating a more data-efficient path toward practical, non-invasive speech BCIs.




