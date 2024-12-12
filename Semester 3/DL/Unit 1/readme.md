Here’s a detailed breakdown of **Unit 1 topics** with examples, use cases, and applications:  

---

## **Unit 1: Foundations of Deep Learning**

---

### **1. Machine Learning vs. Deep Learning**
#### **Machine Learning (ML):**
- Subset of AI that uses algorithms to find patterns in data and make predictions.
- Relies on structured data and requires feature engineering by humans.  
- **Example**: Predicting house prices using features like location, size, and age.  
- **Applications**: Fraud detection, email spam filtering, and recommendation systems.

#### **Deep Learning (DL):**
- Subset of ML that uses neural networks to mimic the human brain.
- Automatically extracts features from unstructured data (e.g., images, audio, text).
- **Example**: Recognizing faces in photos.  
- **Applications**: Autonomous driving, voice assistants, and natural language processing (NLP).

#### **Comparison Table:**

| **Aspect**          | **Machine Learning**             | **Deep Learning**            |
|---------------------|----------------------------------|------------------------------|
| **Feature Engineering** | Required (manual)               | Automatic                    |
| **Data Dependency**  | Works with small datasets        | Requires large datasets      |
| **Computation**      | Less intensive                  | High (needs GPUs/TPUs)       |
| **Use Case**         | Predictive modeling             | Image/speech recognition     |

---

### **2. Basics of Neural Networks - Inspiration from Biological Neurons**
- Neural networks are modeled after the human brain's structure.
- **Biological Neuron**:  
  - Dendrites receive signals, the soma (cell body) processes them, and axons transmit them to other neurons.  
- **Artificial Neuron**:
  - Inputs (like dendrites), weights (importance of inputs), activation function (processes signals), and output.  
- **Example**: Predicting weather conditions based on humidity, temperature, and pressure.

---

### **3. Basics of TensorFlow - Data Structures in TensorFlow**
#### **TensorFlow**:
- Open-source library for deep learning and numerical computation.  
- Uses **tensors**, which are multidimensional arrays, as its core data structure.
#### **Data Structures**:
- **Scalar**: Single value (e.g., a number).  
- **Vector**: 1D array (e.g., [1, 2, 3]).  
- **Matrix**: 2D array (e.g., [[1, 2], [3, 4]]).  
- **Higher Dimensions**: Tensors with 3D or more (e.g., images with RGB channels).

#### **Example in TensorFlow**:
```python
import tensorflow as tf
# Creating a tensor
tensor = tf.constant([[1, 2], [3, 4]])
print(tensor)
```

#### **Applications**:
- Building and training neural networks for image classification, NLP, and more.

---

### **4. Single Neuron Model, Perceptron**
#### **Single Neuron Model**:
- Simplest form of a neural network.  
- **Steps**:
  1. Takes input data.
  2. Multiplies it with weights.
  3. Adds a bias term.
  4. Applies an activation function.

#### **Perceptron**:
- Basic model introduced by Frank Rosenblatt.
- Can classify linearly separable data.  
- **Example**: Separating apples and oranges based on weight and color.  
- **Limitations**: Cannot classify non-linear data like XOR.

---

### **5. Linear and Non-Linear Classifier Using Neural Networks**
#### **Linear Classifier**:
- Decision boundary is a straight line.
- **Example**: Predicting pass/fail based on marks.
- **Limitations**: Cannot handle non-linear patterns.

#### **Non-Linear Classifier**:
- Decision boundary can be curves or complex shapes.  
- Achieved using multiple layers and non-linear activation functions.  
- **Example**: Classifying images of cats and dogs.

---

### **6. Role of Activation Functions**
- Adds non-linearity to the model, enabling it to learn complex patterns.  
- **Common Activation Functions**:
  1. **ReLU**: \(\text{max}(0, x)\). Commonly used in CNNs.  
  2. **Sigmoid**: Outputs probabilities (values between 0 and 1).  
  3. **Tanh**: Outputs values between -1 and 1.  
- **Example**: Predicting whether an email is spam (Sigmoid) or recognizing handwritten digits (ReLU).

---

### **7. Layers in Neural Networks**
- **Input Layer**: Takes raw data as input.
- **Hidden Layers**: Extract features and patterns.
- **Output Layer**: Provides final predictions.  
- **Example**: In image classification:
  - Input: Raw pixel data.
  - Hidden: Extract edges, textures.
  - Output: Classifies objects (e.g., dog, cat).

---

### **8. Feed Forward and Backpropagation**
#### **Feed Forward**:
- Data moves from input to output layer in a forward direction.  
- **Example**: Passing image data through layers for prediction.

#### **Backpropagation**:
- Algorithm used to update weights to minimize error.  
- Steps:
  1. Compute error (loss function).
  2. Adjust weights using gradient descent.

---

### **9. Loss Functions - Binary Cross Entropy and Categorical Cross Entropy**
#### **Binary Cross Entropy**:
- Used for binary classification tasks.  
- ![image](https://github.com/user-attachments/assets/2d291471-84d7-4eb4-98b7-c5a8c7ef7a76)

- **Example**: Spam vs. Not Spam emails.

#### **Categorical Cross Entropy**:
- Used for multi-class classification tasks.  
![image](https://github.com/user-attachments/assets/866e47aa-b6b3-4aa8-bfd1-72e1eecc4cec)
- **Example**: Classifying images of animals into categories like dog, cat, horse.

---

### **Real-World Applications**
1. **Autonomous Vehicles**:
   - Uses neural networks for object detection and decision-making.
2. **Healthcare**:
   - Diagnosing diseases from medical images using CNNs.
3. **Finance**:
   - Fraud detection using classification models.
