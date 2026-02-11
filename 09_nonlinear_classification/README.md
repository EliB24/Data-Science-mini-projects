# Make Moons - Linear vs Deep Neural Networks
This project explores how different neural network architectures perform on a synthetic two-dimensional classification dataset  
The goal is to compare a simple linear model with deeper neural networks and understand how model complexity affects performance

---

## Project Overview

The dataset is generated using `make_moons` from scikit-learn.

It contains:

- Two input features (x1, x2)
- Two classes (binary classification)
- A non-linear structure with added noise

### Models Implemented

1. **Single Neuron (Linear Baseline)**
   - One dense layer with sigmoid activation
   - Represents a linear classifier

2. **Deep Neural Network**
   - Hidden layers with ReLU activation
   - Learns non-linear feature transformations

3. **Regularized DNN**
   - Dropout layers
   - EarlyStopping to prevent unnecessary training

---

## Files Included

- **09_nonlinear_classification.ipynb** - main Jupyter Notebook 
- **README.md** - project description

---

## Technologies Used

- **Python 3**  
- **NumPy**
- **scikit-learn** - dataset generation, preprocessing, model training, and evaluation 
- **TensorFlow / Keras** - building and training neural network models 
- **matplotlib** - visualization
- **Jupyter Notebook / JupyterLab**

---

## Results

- The linear baseline struggles to model the curved structure of the data
- The deep neural network achieves higher validation accuracy
- Visualization of predicted probabilities shows that deeper models learn non-linear decision boundaries
- Regularization improves stability and generalization

---

## How to Run

1. Open `09_nonlinear_classification.ipynb` in Jupyter Notebook or JupyterLab  
2. Make sure all required libraries are installed
4. Run the cells from top to bottom

*The dataset is generated automatically inside the notebook*
