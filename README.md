# Handwritten Digit Classifier (MNIST)

A minimal fully-connected neural network that reaches ≈98 % test accuracy on the classic MNIST digit-recognition task.

## 1. Model architecture
| Layer | Units | Activation |
|-------|-------|------------|
| Input | 784 | – |
| Dense   | 128 | ReLU |
| Dense   | 10  | Softmax |

Total trainable parameters: 101,770.

## 2. Training details
* Dataset: MNIST (60,000 train + 10,000 test grayscale 28×28 digits)  
* Optimizer: Adam, learning-rate 0.01  
* Loss: SparseCategoricalCrossentropy (from logits)  
* Epochs: 20  
* Achieved metrics (test set): **accuracy 0.969 • loss 1.041**

## 3. Quick-start (Install dependencies)
```
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
```

