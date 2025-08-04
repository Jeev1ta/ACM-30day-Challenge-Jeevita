In this task, I learned how to build a simple brain-like model using PyTorch called an MLP (Multilayer Perceptron). This model helps predict if a person will finish a book or drop it, using book details like how long it is and how people rated it.

# Data Preparation
- Loaded the book data from books.csv
- Kept only 3 useful columns (average rating, ratings count, review count)
- Converted the rating into a label (1 or 0)
- Scaled the features so the model trains better
- Split the data into training (80%) and testing (20%)

# Model Design
- Built a neural network (MLP) from scratch using PyTorch
  - 1 input layer with 3 values
  - 1 hidden layer with 16 neurons and ReLU activation
  - 1 output neuron with Sigmoid (since we want a binary result: 0 or 1)

# Training the Model
- Ran for 20 training cycles (epochs)
- In each cycle:
  - Model predicts based on training data
  - Calculates error (loss)
  - Adjusts weights using an optimizer (Adam)
- Plotted the training loss to make sure it's going down

# Evaluation
- Tested the model on unseen data (test set)
- Predicted whether users would drop or finish the book
- Measured performance using:
  - Accuracy → % of total predictions that were correct
  - Precision → How many predicted “finish” books were actually finished
  - Recall → How many actual “finished” books were correctly predicted
  - F1 Score → A balance between precision and recall
