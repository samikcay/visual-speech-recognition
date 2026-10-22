# Visual Speech Recognition from Lip Movements

Term project for Introduction to Image Processing.

## Project scope

Develop a word-level visual speech recognition system using a CNN-LSTM network. The target vocabulary is approximately **30 English words**. The final vocabulary and dataset subset will be defined during data preparation.

- **Input:** A short, silent video clip containing one target word.
- **Image processing:** Mouth-region detection and cropping, grayscale conversion, resizing, and intensity normalization.
- **Models:** A CNN baseline with averaged frame features, followed by a CNN-LSTM model for temporal sequence classification.
- **Output:** The predicted word from the selected vocabulary.
- **Evaluation:** Accuracy, macro F1-score, and a confusion matrix, using separate speakers for training, validation, and testing.

## Initial milestone

Prepare a small labeled dataset sample, extract word-level clips using the supplied time alignments, and visually verify the processed mouth-region frame sequences.

Repository initialized; data preparation is the first implementation milestone.

## Version control

Source code, notebooks, reproducible configuration, and vocabulary definitions belong in Git. Downloaded datasets, videos, generated frames, model checkpoints, experiment outputs, virtual environments, and secrets are excluded by `.gitignore`.

Use `data/` or `datasets/` for local datasets. Small documentation images can be tracked outside those directories. Environment-variable templates can be tracked as `.env.example`; actual `.env` files remain local.

## References

- [GRID Audio-Visual Speech Corpus](https://zenodo.org/records/3625687)
- [Combining Residual Networks with LSTMs for Lipreading](https://arxiv.org/abs/1703.04105)
- [LipNet: End-to-End Sentence-level Lipreading](https://arxiv.org/abs/1611.01599)
