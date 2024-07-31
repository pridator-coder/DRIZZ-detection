# Driver Drowsiness Detection Using CNN (VGG19)

This project focuses on detecting driver drowsiness using Convolutional Neural Networks (CNN) with the VGG19 architecture. The model is trained to classify images into four categories: closed eyes, open eyes, yawning, and no yawn. By identifying these states, the system aims to provide a reliable method to detect drowsiness and prevent potential accidents due to fatigue.

## Project Details

### Notebook

For detailed steps and code execution, you can view the Kaggle notebook [here](https://www.kaggle.com/code/priyanshukumar45/driver-drowsiness).

### Model Architecture

The model leverages the VGG19 architecture, pre-trained on the ImageNet dataset. We use transfer learning to benefit from the powerful feature extraction capabilities of VGG19. The base model's layers are frozen, and custom layers are added on top for classification.

### Results

The model achieves an impressive testing accuracy of **97.46%**. Here are the detailed metrics:

|               | precision | recall | f1-score | support |
|---------------|-----------|--------|----------|---------|
| closed_eye    | 1.00      | 0.99   | 1.00     | 109     |
| open_eye      | 0.99      | 1.00   | 1.00     | 109     |
| yawning       | 0.99      | 0.92   | 0.95     | 109     |
| no_yawn       | 0.92      | 0.99   | 0.95     | 106     |

|    accuracy   |           |        | 0.97     | 433     |
|   macro avg   | 0.98      | 0.97   | 0.97     | 433     |
| weighted avg  | 0.98      | 0.97   | 0.97     | 433     |

### Dataset

The dataset used for training and testing the model is available on Kaggle: [Yawn Eye Dataset New](https://www.kaggle.com/datasets/serenaraju/yawn-eye-dataset-new).



## How to Use

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/driver-drowsiness-detection.git
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the training script:
    ```bash
    python train.py
    ```

4. Test the model:
    ```bash
    python test.py
    ```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
