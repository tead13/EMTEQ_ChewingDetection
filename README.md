# Chewing Detection with Deep Learning

This repository contains a project developed for the course **Intelligent Information Systems**.

The project focuses on chewing detection using deep learning techniques applied to sensor data collected from Emteq smart glasses. The goal is to automatically detect chewing activity from wearable sensor signals and evaluate how different deep learning and transfer learning approaches perform across different versions of smart glasses.

## Project Description

Chewing detection is an important task in eating behaviour analysis and dietary monitoring. In this project, the complete workflow was covered, starting from data collection, data organization and preprocessing, to training and evaluating different deep learning models.

The data were collected using Emteq S11 smart glasses from multiple participants. The recordings include sensor signals related to facial and motion activity, which were used to distinguish chewing from non-chewing behaviour. In addition to the newly collected S11 dataset, older data from a previous generation of Emteq smart glasses were also used in order to explore transfer learning between different hardware versions.

The main modeling approach is based on 1D Convolutional Neural Networks, which are suitable for multichannel time-series sensor data. Several experimental setups were tested, including models trained only on new data, models trained on old data, zero-shot transfer, fine-tuning, joint training, and transfer learning between old and new datasets.

## Main Goals

The main goals of the project are:

- to collect and organize sensor data from smart glasses;
- to preprocess and prepare the data for deep learning;
- to train different 1D CNN models for chewing detection;
- to compare different training strategies;
- to evaluate transfer learning between older and newer Emteq glasses;
- to analyze model performance using standard classification metrics.

## Dataset

The new dataset was collected using **Emteq S11 smart glasses** from 42 participants. The recordings followed a structured protocol and included phases such as calibration, reading, and eating. For the chewing detection task, the focus was mainly on the eating phase, where chewing and non-chewing activities were labeled and used for model training and evaluation.

Previously recorded data from an older version of Emteq smart glasses were also used to support transfer learning experiments. This allowed comparison between models trained on old data, new data, and combinations of both datasets.

## Methods

The project includes the following main steps:

1. Data collection using Emteq smart glasses.
2. Data organization by participants.
3. Preprocessing and cleaning of sensor signals.
4. Feature selection from relevant sensor modalities.
5. Normalization of input data.
6. Segmentation into fixed-length time windows.
7. Training of 1D CNN models.
8. Evaluation of different training and transfer learning approaches.

## Models and Experiments

Several model configurations were evaluated:

- model trained only on old data;
- model trained only on new S11 data;
- zero-shot transfer between datasets;
- partial fine-tuning;
- full fine-tuning;
- joint training using old and new data;
- transfer learning between different smart glasses versions.

The main architecture used in the project is a **1D Convolutional Neural Network**, designed for time-series classification using wearable sensor data.

## Results

The results showed that the model trained directly on the new S11 dataset achieved the best overall performance. Transfer learning approaches significantly improved performance compared to zero-shot transfer, showing that adaptation between different hardware versions is important.

The experiments demonstrated that deep learning, especially 1D CNN models, can be successfully applied to chewing detection using smart glasses sensor data. The results also showed that transfer learning can help reduce the performance gap between data collected from different versions of wearable devices.
