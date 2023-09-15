[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
![GitHub pull requests](https://img.shields.io/github/issues-pr/suvadeepmaiti/EEG_Sleep_Stage_classification)
![GitHub issues](https://img.shields.io/github/issues/suvadeepmaiti/EEG_Sleep_Stage_classification)

# A Deep Dive into Sleep: Single-Channel EEG-Based Sleep Stage Classification with Model Interpretability
This repository contains code, results, and dataset links for our arxiv paper titled ***A Deep Dive into Sleep: Single-Channel EEG-Based Sleep Stage Classification with Model Interpretability***. 📝
>**Authors:** <a name="myfootnote1"><sup>1</sup></a>Shivam Kumar Sharma, <a name="myfootnote1"><sup>1</sup></a>Suvadeep Maiti, S.Mythirayee, Srijithesh Rajendran, Bapi Raju

<sup>[1](#myfootnote1)</sup>Equal contribution

>**More details on the paper can be found [here](http://arxiv.org/abs/2309.07156).**
> **Raise an issue for any query regarding the code, paper, or for any support.**

## Table of contents
- Introduction
- Highlights
- Results
- Dataset
- Getting started
- Getting the weights
- License and Citation

## Introduction 🔥

>Sleep, a fundamental physiological process, occupies a significant portion of our lives. Accurate classification of sleep stages serves as a crucial tool for evaluating sleep quality and identifying probable sleep disorders. This work introduces a novel methodology that utilises a SE-Resnet-BiLSTM architecture to classify sleep into five separate stages. The classification process is based on the analysis of single-channel electroencephalograms (EEGs). The framework that has been suggested consists of two fundamental elements: a feature extractor that utilizes SE-ResNet, and a temporal context encoder that use stacks of Bi-LSTM units.The effectiveness of our approach is substantiated by thorough assessments conducted on three different datasets, namely SLeepEDF-20, SleepEDF78, and SHHS. Notably, we introduce the utilization of 1D-GradCAM visualization to shed light on the decisionmaking process of our model in the realm of sleep stage classification. This visualization method not only provides valuable insights into the model’s classification rationale but also aligns its outcomes with the annotations made by sleep experts. 

## Highlights ✨

- A supervised model trained on Electroencephalography (EEG) data beating the current SOTA models 💥.
- Complete pre-processing pipeline, augmentation, and training scripts are available for experimentation.
- Pre-trained model weights are provided for reproducibility.

## Results :man_dancing:

> Linear evaluation results on Sleep-EDF-20, Sleep-EDF-78 and SHHS datasets.

|          | Accuracy | κ | Macro F1-score |
| -------- | ------------- | ------------- | ------------- |
| Sleep-EDF-20| 87.5 | 0.82 | 82.5 |
| Sleep-EDF-78 | 83.8 | 0.77 | 78.9 |
| SHHS| 76.75 | 0.83 | 81.9 |


<!--t-SNE visualization using our method shows clear clusters and captures the sleep-staging progression observed clinically.-->

<!--<img src="/images/tsne.jpg" width="750">-->

>1D-GradCAM visualization of raw EEG epochs along with sleep micro-structures shown in green boxes.
<img src="/images/gradcam.jpg" width="750">

## Getting started 🥷
#### Setting up the environment
TODO
#### What each file does
TODO
#### Training the model
TODO
#### Testing the model
TODO
#### Logs and checkpoints
- The logs are saved in `logs/` directory.
- The model checkpoints are saved in `checkpoints/` directory.

## Getting the weights :weight_lifting:
TODO

## License and Citation 📰
Please cite the following paper if you have used this code:
```
@misc{sharma2023deep,
      title={A Deep Dive into Sleep: Single-Channel EEG-Based Sleep Stage Classification with Model Interpretability}, 
      author={Shivam Sharma and Suvadeep Maiti and S. Mythirayee and Srijithesh Rajendran and Bapi Raju},
      year={2023},
      eprint={2309.07156},
      archivePrefix={arXiv},
      primaryClass={eess.SP}
}
