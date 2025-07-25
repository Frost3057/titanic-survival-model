# Titanic Survival Prediction Model

This project aims to predict the survival of passengers on the RMS Titanic using a machine learning model. The model is built with PyTorch and trained on the classic Titanic dataset from Kaggle.

## Dataset

The dataset is sourced from the [Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic) competition on Kaggle. It is split into two files:

- `train.csv`: Contains the training data with features and the "Survived" label.
- `test.csv`: Contains the test data with features, but without the "Survived" label.
- `gender_submission.csv`: An example of the required submission format.

The features used for training the model are: `Pclass`, `Sex`, `Age`, `Cabin`, and `Parch`.

## Model Architecture

A neural network is implemented using PyTorch to classify whether a passenger survived. The architecture is as follows:

- **Input Layer:** Takes 5 features as input.
- **Hidden Layer 1:** Linear layer with 8 neurons, followed by a ReLU activation function.
- **Hidden Layer 2:** Linear layer with 16 neurons, followed by a ReLU activation function.
- **Hidden Layer 3:** Linear layer with 8 neurons, followed by a ReLU activation function.
- **Output Layer:** A single linear neuron to output the survival prediction.

The model uses Binary Cross-Entropy with Logits Loss (`BCEWithLogitsLoss`) as the loss function and Stochastic Gradient Descent (`SGD`) as the optimizer.

## Technologies Used

- **Python**
- **PyTorch:** For building and training the neural network.
- **Pandas:** For data loading and manipulation.
- **NumPy:** For numerical operations.
- **Matplotlib:** For data visualization.
- **Jupyter Notebook:** For interactive development and model training.

## How to Run

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Frost3057/titanic-survival-model.git
    cd titanic-survival-model
    ```

2.  **Install dependencies:**
    Make sure you have Python and pip installed. Then, install the required libraries:
    ```bash
    pip install torch numpy matplotlib pandas jupyter
    ```

3.  **Download the dataset:**
    Download the `train.csv` and `test.csv` files from the [Kaggle competition page](https://www.kaggle.com/c/titanic/data) and place them in a `titanic` subfolder.

4.  **Run the Jupyter Notebook:**
    Launch Jupyter Notebook and open `main.ipynb`:
    ```bash
    jupyter notebook main.ipynb
    ```

5.  **Execute the cells:**
    Run the cells in the notebook sequentially to load the data, preprocess it, define the model, train it, and evaluate its performance.
