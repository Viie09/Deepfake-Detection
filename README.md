# Deepfake Detection: DeepTruth

## Introduction
Deepfake technology presents significant challenges to content authenticity, threatening digital trust. Our project, **DeepTruth**, focuses on detecting deepfake videos using an integrated approach that combines machine learning and deep learning techniques. The goal is to develop a robust detection system to address the growing threat of manipulated media.

## Features
- Utilizes **ResNeXt** for spatial feature extraction.
- Implements **Temporal Convolutional Networks (TCN)** for analyzing temporal patterns.
- Leverages **XGBoost** for reliable classification.
- Employs data augmentation strategies to address dataset imbalance.
- Trained and evaluated on the **Celeb-DF v2** dataset.

## Technologies Used
- **Python**
- **PyTorch**
- **XGBoost**
- **OpenCV**
- **MTCNN** for face detection
- **Albumentations** for data augmentation

## Dataset
The project utilizes the **Celeb-DF v2** dataset, which includes:
- **590 real videos**
- **5,639 deepfake videos**
- Videos processed at 30 frames per second with an average length of 13 seconds.

## Methodology
### Architecture
1. **ResNeXt**:
   - Extracts spatial features from individual video frames.
   - Utilizes grouped convolutions to enhance efficiency.

2. **Temporal Convolutional Networks (TCN):**
   - Captures temporal patterns in video sequences.
   - Efficiently handles long-term dependencies.

3. **XGBoost:**
   - Combines spatial and temporal features for final classification.

### Preprocessing
- Face detection and cropping using **MTCNN**.
- Data augmentation techniques including flipping, rotation, and color jittering.
- Normalization based on ImageNet dataset statistics.

### Performance Metrics
- **Accuracy**: 99.52%
- **Precision**: 99.63%
- **Recall**: 99.50%
- **F1-Score**: 99.50%

## How to Run
1. Clone the repository:
   ```bash
   git clone git@github.com:Viie09/Deepfake-Detection.git
   cd Deepfake-Detection
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the main script:
   ```bash
   python main.py
   ```

## Results
The system achieves state-of-the-art performance on the Celeb-DF v2 dataset, outperforming existing models in terms of accuracy and reliability.


## Contributors
- **Reema Mohammed BinSaeedan**
- **Dalal Mohammed Majrishi**
- **Sadeem Saad Alnfeisah**
- **Lulu Fahad Altuwijri**

## Supervisor
**Dr.Manal Alsabhan**

## Acknowledgments
We would like to express our gratitude to **Imam Mohammad Ibn Saud Islamic University** for providing us with the resources and guidance to complete this project. Special thanks to our supervisor, **Dr.Manal Alsabhan**, for her continuous support and mentorship throughout the project.



