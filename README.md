****Deep Learning Based Writer Identification System****

A deep learning-based writer identification system that analyzes handwriting samples and predicts the corresponding writer using multiple state-of-the-art computer vision architectures.
This project explores and benchmarks CNNs, EfficientNet, SE-ResNet, and Vision Transformers on large-scale handwriting datasets under a writer-independent evaluation setup.

---
**Overview**

Writer identification is an important problem in document forensics, signature verification, historical manuscript analysis, and biometric authentication. Traditional approaches rely heavily on handcrafted features, whereas modern deep learning architectures can automatically learn robust writer-specific representations from handwriting samples.

This project presents a comparative study of multiple deep learning architectures for writer identification using large-scale handwriting datasets. The system includes preprocessing pipelines, model training workflows, benchmarking utilities, Grad-CAM visualizations, and writer-independent evaluation methodologies.

---
**Features**
- Writer-independent training and evaluation
- Comparative benchmarking of multiple DL architectures
- CNN, EfficientNet, SE Attention, and Vision Transformer implementations
- Automated preprocessing and augmentation pipeline
- Grad-CAM based model interpretability
- Accuracy and performance visualization
- Modular and scalable training pipeline
- Research-oriented experimentation workflow

---
**Models Used**
| Model |	Purpose |
| ----- | ------- |
CNN	| Baseline feature extraction
EfficientNet | Efficient deep feature learning
SE Attention	| Channel attention-based representation learning
Vision Transformer (ViT) |	Global context modeling

---
**Siamese Network Flowchart**

<img width="512" height="280" alt="image" src="https://github.com/user-attachments/assets/c98c27fb-b137-44f7-8a55-52370841052c" />

---
**Tech Stack**
- Python
- PyTorch
- OpenCV
- NumPy
- Scikit-learn
- Matplotlib
- Pandas
- TensorFlow
  
---
**Dataset**

The project is trained and evaluated on large-scale handwriting dataset namely IAM Handwriting Dataset
Note: Datasets are publicly available and are not included in this repository due to licensing restrictions.
Sample Images:
<img width="812" height="176" alt="image" src="https://github.com/user-attachments/assets/85913939-00fb-48a9-b6a1-ae2ed4c6e945" />

---
**Preprocessing Pipeline**

The preprocessing workflow includes:

- Grayscale conversion
- Noise reduction
- Normalization
- Image resizing
- Data augmentation
- Batch generation for training
- Training Pipeline

The system supports:

- Multi-model experimentation
- Configurable hyperparameters
- GPU acceleration
- Checkpoint saving
- Early stopping
- Learning rate scheduling

Example:
``` bash
python train.py --model efficientnet --epochs 50 --batch_size 32
```
---
**Evaluation**

The project uses a writer-independent evaluation strategy to ensure robust generalization on unseen writers.

Evaluation metrics include:

- Accuracy
- AUC-ROC Score
- Cross Entropy Loss

Example:
```bash
python evaluate.py --model vit
```
**Grad-CAM Visualization**

Grad-CAM based interpretability is used to visualize important handwriting regions influencing model predictions.

This helps in:

- understanding model behavior
- improving explainability
- validating learned writer-specific patterns
  
---
**Sample Outputs**
- Grad-CAM Visualization


<img width="250" height="180" alt="image" src="https://github.com/user-attachments/assets/40b6e97d-5034-4b22-acb8-5a1c9a2167f8" /><img width="250" height="180" alt="image" src="https://github.com/user-attachments/assets/23857294-639a-4fb5-8bdf-8bfa4c8fc582" />

- Training Curves

<img width="350" height="250" alt="image" src="https://github.com/user-attachments/assets/0f6ad471-ee97-42f5-9260-63b4cf72b319" />     <img width="350" height="250" alt="image" src="https://github.com/user-attachments/assets/0f2dd96e-3666-4432-9f4e-d98789d22ca2" />
<img width="350" height="250" alt="image" src="https://github.com/user-attachments/assets/415bcb9f-f6be-4fac-90f8-1affff771e88" />     <img width="350" height="250" alt="image" src="https://github.com/user-attachments/assets/03b3e80f-b219-42ff-8f6a-40ed7ce0dc20" />





---
**Installation**

- Clone the repository:
```bash
git clone https://github.com/your-username/writer-identification-system.git
cd writer-identification-system
```

- Install dependencies:
```bash
pip install -r requirements.txt
```

- Inference

Run inference on a handwriting sample:
``` bash
python inference.py --image sample.jpg
```
---
**Research Contribution**

This project was developed as part of a research study on deep learning-based writer identification systems. Research paper under preparation/submission to CVIT Conference.

---
**Future Improvements**
- Self-supervised handwriting representation learning
- Lightweight deployment models
- Cross-dataset generalization
- Real-time inference optimization
- Hybrid CNN-Transformer architectures
---
**Author**

Bitra Sri Pragna
- Computer Science Undergraduate
- Machine Learning & Software Engineering Enthusiast

---
**License**

This project is intended for educational and research purposes.
