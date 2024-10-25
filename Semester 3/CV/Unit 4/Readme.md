> The various topics inside unit 4 has been sorted into categories.
---

### **Image Feature Extraction**

1. **Quantitative Feature Computation**:
   - Quantitative features are numeric descriptors that summarize specific aspects of the image, such as size, shape, or color intensities.
   - Useful in creating measurable attributes for model input.

2. **Shape or Orientation Feature Extraction**:
   - **Shape Features**: Describe geometric properties like area, perimeter, or aspect ratio of objects in an image.
   - **Orientation Features**: Describe the alignment of objects within an image. Commonly used metrics include angles, curvature, and directionality.

3. **Statistical or Texture Feature Extraction**:
   - **Texture Features**: Capture patterns and variations in intensity or color across an image, using metrics like contrast, homogeneity, and entropy.
   - **Statistical Features**: Use histogram-based metrics (e.g., mean, variance) or GLCM (Gray Level Co-occurrence Matrix) for detailed texture analysis.

---

### **Lab Work for Feature Extraction and Reduction**

4. **Lab 10: Extracting Shape and Texture Features**:
   - In this lab, you would use image processing libraries to segment an image, then apply methods to calculate features related to shape (e.g., contour analysis) and texture (e.g., GLCM).

5. **Transform Domain Feature Extraction**:
   - Transform domain methods, like Fourier Transform or Wavelet Transform, analyze images in a frequency domain, capturing patterns that may not be visible in the spatial domain.

6. **Feature Visualization**:
   - Visualizes features to assess patterns or clusters within the data.
   - Techniques like t-SNE or PCA can project high-dimensional features into 2D or 3D space for easier interpretation.

7. **Feature Reduction and Scaling**:
   - **Reduction**: Techniques like PCA or LDA reduce the dimensionality of features, retaining only the most important ones.
   - **Scaling**: Normalizes features (e.g., standardizing to zero mean and unit variance) to improve model performance and convergence.

8. **Lab 11: Performing Feature Reduction**:
   - This lab involves applying algorithms like PCA on extracted features to select the most informative ones, reducing computational load without sacrificing accuracy.

---

### **Machine Learning Model Building and Evaluation**

9. **Overview of Machine Learning Models**:
   - Covers different model types for image-based tasks:
     - **Classification models**: SVM, Decision Trees, KNN.
     - **Ensemble methods**: Random Forest, Gradient Boosting.
     - **Neural networks**: CNNs for image-specific tasks.

10. **Machine Learning Model Building on Extracted Features**:
    - The process of training models on image features (shape, texture) to create predictive systems.
    - Models are built by feeding extracted features into ML algorithms for supervised learning tasks.

11. **ML Model Evaluation and Tuning**:
    - **Evaluation Metrics**: Accuracy, precision, recall, F1-score, and ROC-AUC.
    - **Tuning**: Optimizing model hyperparameters using techniques like Grid Search or Random Search.

12. **Lab 12: Building a Predictive Model on Extracted Features**:
    - In this lab, you’ll use the extracted features to train, evaluate, and optimize an ML model.
    - Steps include feature selection, model training, hyperparameter tuning, and evaluating model performance.

---
