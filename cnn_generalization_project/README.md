# CIFAR-10 -  CNN Generalization Study
The goal of this project is to explore how architectural improvements and training strategies affect model generalization in image classification  
I start with a simple basic CNN and then improve it using modern deep learning techniques  
Finally, I analyze the model's errors to understand the patterns of failure  

This project demonstrates:

- CNN architecture design
- Regularization techniques
- Training optimization
- Validation strategy
- Error analysis workflow 

---

## Project Overview

### Dataset

Dataset: **CIFAR-10**

- 60 000 images
- 32×32 RGB
- 10 classes:
  airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck

The dataset is loaded directly from `tensorflow.keras.datasets`

---

### 01 - Baseline Model

#### Architecture
Conv - MaxPool - Conv - MaxPool - Conv - Flatten - Dense - Softmax

#### Training Setup
- Optimizer: Adam
- Loss: Sparse Categorical Crossentropy
- Epochs: 12
- Batch size: 64

#### Results
- Test Accuracy ≈ 71%

#### Observations
- Model starts overfitting after several epochs
- Accuracy of validation stabilizes at the initial stage
- Some classes (cat, deer, dog) are difficult

---

### 02 - Improved Model

Improvements Applied:  

1. Data Augmentation:  
- Random horizontal flip
- Random rotation
- Random zoom

Used only during training

2. Batch Normalization: Improves gradient flow and training stability  
3. Dropout: Reduces overfitting  
4. GlobalAveragePooling: Replaces Flatten to reduce parameters  
5. Callbacks: EarlyStopping, ReduceLROnPlateau  

#### Training Setup
- Learning rate scheduling
- Up to 40 epochs
- Best weights restored

#### Results
- Test Accuracy ≈ 82%
- Better class balance
- Reduced overfitting

#### Improvement
+11% absolute accuracy gain over baseline

---

### 03 - Error Analysis

After improving performance, i analyze model failures

#### Analysis Includes

- Confusion matrix
- Per-class accuracy
- Misclassified examples
- High-confidence errors
- Export of error cases to CSV

#### Key Insights

- Cats vs Dogs remain confusing  
- Some errors occur even with >99% confidence  
- Certain classes (frog, truck) are learned very well  
- Visual similarity strongly affects mistakes

---

## Experimental approach

To ensure an objective comparison:

- Use the same data partitioning
- Apply the same normalization
- Evaluate using the same metrics
- Only change the architecture or training strategy

This approach allows to identify the impact of changes in architecture and training strategy on the results

---

## Files Included

- **01_cifar10_baseline.ipynb** - baseline CNN implementation  
- **02_cifar10_improvements.ipynb** - architecture and training improvements  
- **03_error_analysis.ipynb** - performance and error diagnostics  
- **results/** - project artifacts:
  - trained models  
  - evaluation metrics  
  - plots and confusion matrices  
  - exported error analysis results  
- **requirements.txt** - project dependencies  
- **README.md** - full project overview

---

## Technologies Used

- **Python 3** 
- **TensorFlow / Keras** - CNN architecture, training loop, callbacks, model serialization
- **NumPy** - tensor manipulation and probability processing
- **pandas** - experiment tracking and structured result export
- **scikit-learn** - evaluation utilities (confusion matrix, data splitting)
- **Matplotlib / Seaborn** - visualization and diagnostics
- **pathlib** - reproducible file handling

---

## How to Run

1. Clone or download this repository  
2. Open the project folder in Jupyter Notebook or JupyterLab  
3. Make sure all required libraries from `requirements.txt` are installed  
4. Run the notebooks in order:

   - `01_cifar10_baseline.ipynb`
   - `02_cifar10_improvements.ipynb`
   - `03_error_analysis.ipynb`

*The CIFAR-10 dataset is loaded automatically from TensorFlow/Keras*
