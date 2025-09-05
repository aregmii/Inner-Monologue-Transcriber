# Mission Statement

To push the frontier of inner monologue transcription by applying modern sequence-to-sequence transformer models to decode sentence-level neural signals from non-invasive EEG. The goal is to create the first open-source benchmark for this task, contributing to technology that could one day restore communication for those who have lost the ability to speak.

# Problem Statement

Decoding speech directly from brain signals is one of the great challenges in neuroscience and AI. While significant progress has been made with invasive methods (ECoG), and impressive classification results exist for non-invasive EEG, a major gap remains in achieving continuous, open-vocabulary decoding with non-invasive technology. This project aims to bridge that gap.

# State of the Art (The Benchmark)

The field of neural speech decoding is defined by a trade-off between signal quality (invasiveness) and task complexity. This project sits at the cutting edge of non-invasive technology.

1. SOTA in Invasive Decoding (ECoG/Microelectrode Arrays):

A Stanford study (Willett et al., 2025) achieved a Word Error Rate (WER) of ~26% for decoding continuous, inner speech. 
More: https://news.stanford.edu/stories/2025/08/study-inner-speech-decoding-device-patients-paralysis

2. SOTA in Non-Invasive Classification (EEG):

With EEG, the primary challenge is the low signal-to-noise ratio. The most relevant and recent work comes from the authors of the Chisco dataset themselves.

The Chisco datasets use a "read then imagine" paradigm, where participants first read a sentence and are then cued to imagine speaking it. This provides a ground-truth label for the internal speech act.

The Benchmark: The paper "How Far Are We From... Non-Invasive Speech BCIs?" (Bao et al.) established the most relevant baseline. They did not attempt full transcription. Instead, they measured the cosine similarity between EEG signal embeddings and text embeddings for a simplified task of distinguishing between just two semantic categories. Their SOTA result was a similarity score of ~0.16 (where 1.0 is a perfect match).

# The Data Scalability Challenge & Opportunity

The most critical finding from the Bao et al. paper is their "non-invasive speech BCI scaling law." Their analysis projects that achieving high-performance, open-vocabulary decoding with current models would require "approximately 15 years’ worth of data from a single participant".

The project's goal is to prove this scaling law can be beaten with a more intelligent approach. It will be the first to perform end-to-end, sentence-level transcription on the Chisco-2.0 dataset. The mission is to establish the first credible WER/BLEU benchmark and demonstrate that a novel feature representation can make non-invasive speech decoding feasible without requiring decades of data.