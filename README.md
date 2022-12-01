# Speech Emotion Recognition
Benchmarking the performance of handcrafted features (from openSMILE) and data-driven features (from self-supervised learning based models) on speech emotion recognition task across multilingual datasets 

## Demo files
- `speech_emotion_recognition_demo.ipynb` [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/satvik-dixit/speech_emotion_recognition/blob/main/speech_emotion_recognition_demo.ipynb) A demo containing all steps of speech emotion recoginition using the EmoDB dataset. It includes loading and resampling audio files, extracting metadata, extracting DL based and handcrafted features, speaker normalisation, hyperparameter tuning and getting classification reports for logistic regression, SVM and random forest classification
- `datasets_demo.ipynb` [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/satvik-dixit/speech_emotion_recognition/blob/main/datasets_demo.ipynb) A demo for comparing results obtained using multiple datasets. It includes performing all the steps on the following open source datasets: CaFE (French), EmoDB (German), ShEMO (Persian), RAVDESS (English), CREMA-D (English), SAVEE (British English)

## Datasets
- <a href="http://emodb.bilderbar.info/index-1280.html">EmoDB Dataset</a>
- <a href="https://zenodo.org/record/1478765#.YvyXfexBy3I">Canadian French Emotion (CaFE)</a>
- <a href="https://github.com/mansourehk/ShEMO"> Persian Speech Emotion Detection Dataset (ShEMO) </a>
- <a href="https://zenodo.org/record/1188976#.YvyPHexBy3K">Ryerson Audio-Visual Database of Emotional Speech and Song (RAVDESS)</a>
- <a href="https://github.com/CheyneyComputerScience/CREMA-D">Crowd Sourced Emotional Multimodal Actors Dataset (CREMA-D)</a>
- <a href="http://kahlan.eps.surrey.ac.uk/savee/Database.html">Surrey Audio-Visual Expressed Emotion (SAVEE)</a>

## Results
The recall_macro (%) on different datasets for logistic regression
|Model            | EmoDB | CaFE | ShEMO | CREMA-D | RAVDESS | SAVEE |
|-----------------|-------|------|-------|---------|---------|-------|
|Hybrid BYOL-S    |86.7   |73.4  |55.9   |73.9	   |79.0     |52.9   |
|OpenSMILE compare|82.8   |68.7  |52.0   |70.5	   |70.1	   |63.8   |
|OpenSMILE egemaps|75.6   |61.1  |50.2	 |61.0	   |63.2	   |65.2   |


## References
- https://arxiv.org/abs/2110.03414


