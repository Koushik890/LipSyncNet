
# LipSyncNet: A Deep Learning Approach for Visual Speech Recognition

![Framework of Lip-Reading System](https://github.com/Koushik890/LipSyncNet/blob/main/Framework.png)

**LipSyncNet** is a novel deep learning-based model designed to perform visual speech recognition, particularly in scenarios where audio cues are unavailable or unreliable. The model leverages a combination of 3D-CNNs, EfficientNetB0, and Bi-LSTM layers to effectively process visual data and improve lip-reading accuracy.

## Features

- **3D-CNN for Feature Extraction**: Utilizes 3D Convolutional Neural Networks to capture spatial and temporal features from video sequences.
- **EfficientNetB0 Integration**: Enhances feature extraction with EfficientNetB0, known for its efficient scaling and high-level feature representation.
- **Bi-LSTM for Sequence Modeling**: Processes temporal dependencies in the extracted features, enabling the model to understand the sequential nature of speech.

## Installation and Usage

Clone the repository and install the necessary dependencies:
```
git clone https://github.com/Koushik890/LipSyncNet.git
cd LipSyncNet
pip install -r requirements.txt
```

## Model Architecture

The architecture of LipSyncNet is composed of three main components:

1. **3D-CNN Layer**: Captures volumetric data from the input video frames.
2. **EfficientNetB0**: Provides high-level feature extraction.
3. **Bi-LSTM Layer**: Models the sequential data to predict the speech output.

![Architecture of the proposed 3D-EfficientNetB0-Bi-LSTM-CTC network](https://github.com/Koushik890/LipSyncNet/blob/main/architecture.png)

## Dataset

The model is trained and evaluated on the **GRID corpus**, a comprehensive dataset consisting of 33,000 video samples.

## Results

LipSyncNet achieves a **96.7% accuracy** on the GRID corpus, outperforming previous models by a significant margin. Below is a comparison of the models:

| Model                                 | Accuracy  |
|---------------------------------------|-----------|
| LipSyncNet (Our Model)                | 96.7%     |
| Baseline Model (Xu et al.)            | 89.6%     |
| Previous Best (Margam et al.)         | 91.4%     |

![Loss Graph of 3D-CNN-EfficientNetB0-Bi-LSTM-CTC](https://github.com/Koushik890/LipSyncNet/blob/main/model_loss.png)

## Citation

If you use this code in your research, please cite:

```
@article{Dey2024LipSyncNet,
  title={LipSyncNet: A Novel Deep Learning Approach for Visual Speech Recognition in Audio-Challenged Situations},
  author={Koushik Dey and S A Amutha Jeevakumari},
  journal={IEEE Access},
  year={2024},
  doi={10.1109/ACCESS.2024.3436931}
}
```
## Acknowledgments

Special thanks to the Vellore Institute of Technology, Chennai, for providing the resources and support for this project.
