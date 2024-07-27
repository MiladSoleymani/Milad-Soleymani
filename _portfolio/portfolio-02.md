---
title: "Voice Analysis for CHF Detection"
excerpt: " <img width='350' alt='Screenshot 2024-05-29 at 10 52 36 PM' src='https://github.com/MiladSoleymani/Milad-Soleymani/assets/78655282/2147d685-3721-47cc-a219-1c9de8222213'> <br/> <br/> Working on a groundbreaking research initiative focused on the use of voice <br/> recognition for chronic heart failure (CHF) phenotyping. <br/> [KeyLead Health](https://keyleadhealth.com/), Australia"
collection: portfolio
---

## Overview

This paper presents a novel self-supervised deep learning model for Brain-Computer Interface (BCI) systems, focusing on motor imagery and seizure detection tasks. The model leverages a task-agnostic embedding approach to process Electroencephalography (EEG) signals, enabling efficient BCI decoding without the need for extensive labeled training data.

## Key Contributions

1. **Self-supervised Learning (SSL) Approach**: The proposed model uses SSL to learn embeddings of EEG signals without requiring labeled data, addressing the challenge of limited annotated datasets in BCI research.
2. **Task-agnostic Embedding**: The model generates a common vector representation of EEG signals that can be applied to different BCI tasks, such as motor imagery and seizure detection.
3. **Transferability**: The embedding can be fine-tuned for specific tasks, making the approach versatile and efficient in different BCI applications.
4. **Validation on Multiple Datasets**: The model's effectiveness was demonstrated using two public datasets—BCI Competition IV 2a (for motor imagery) and CHB-MIT (for seizure detection).

## Methodology

### Dataset Description

- **Stage 1**: EEG data from epilepsy monitoring at St Vincent’s Hospital, Melbourne, used for training without task-specific labels.
- **Stage 2**: Public datasets—BCI Competition IV 2a for motor imagery and CHB-MIT for seizure detection—used for model validation.

### Model Architecture

- **Embedder**: Based on a Convolutional Neural Network (CNN) architecture, particularly the EEGNet model, modified to output 128-element vector embeddings of EEG signals.
- **Worker Layer**: Comprises multiple regression components that perform self-supervised tasks, using known signal transformations as pseudo-labels.

### Training and Evaluation

- **Training**: Conducted in a self-supervised manner, with a focus on generating task-agnostic embeddings.
- **Evaluation**: Embeddings were evaluated using clustering techniques, demonstrating the model's ability to distinguish between different BCI states (e.g., seizure vs. no seizure, left vs. right hand movement).

## Results

The proposed model successfully differentiated between binary classes in both motor imagery and seizure detection tasks, validating its task-agnostic and self-supervised learning capabilities.

## Future Work

The paper suggests further exploration into expanding the Worker layer with additional features and applying the model to other BCI tasks to enhance its generalizability.

## References

The paper cites relevant works in the fields of BCI, deep learning, and self-supervised learning, providing a comprehensive background and justification for the chosen approach.
---
