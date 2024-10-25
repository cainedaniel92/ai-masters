> The various topics inside unit 3 has been sorted into 3 categories. 
---

### **Web Scraping and Basic HTML Tags**

1. **Web Scraping**: This is a method to extract large amounts of data from websites, commonly using tools like Beautiful Soup and libraries such as requests in Python.

2. **Basic HTML Tags**:
   - `<html>`, `<head>`, `<body>`: Basic structure tags.
   - `<a>`, `<p>`, `<div>`, `<h1>`, `<img>`, `<table>`: Important tags for text, images, and links that you might need to locate data.

3. **Beautiful Soup**: A Python library used for parsing HTML and XML documents, making it easier to navigate the DOM and find tags or data within them.

4. **Scraping an HTML Page**:
   - Use `requests` to retrieve the page content.
   - Parse HTML with Beautiful Soup.
   - Use methods like `find()` or `find_all()` to locate specific tags/data.
   
5. **Scraping an E-commerce Site**:
   - Identify the HTML structure of the site.
   - Look for elements like product names, prices, and images.
   - Be cautious of ethical and legal aspects (check the site’s robots.txt).

6. **Retrieve Data with API**:
   - APIs allow structured access to data without HTML parsing.
   - Use libraries like `requests` to send HTTP requests and retrieve JSON responses.

---

### **Language Modeling Concepts**

7. **Skip Gram Model**:
   - A word2vec model that predicts context words given a target word.
   - Works well for generating word embeddings in NLP by maximizing similarity between words appearing in similar contexts.

8. **N-Gram**:
   - A contiguous sequence of 'n' items (words) in a text.
   - Used to predict the next word based on the previous `n-1` words (e.g., bigram for two words, trigram for three).
   
9. **Document Similarity**:
   - Measures the similarity between two documents.
   - Techniques: Cosine similarity, Jaccard similarity, and word embeddings.

---

### **Deep Learning Models and Sequence Modeling**

10. **Sequence Modeling**:
    - Involves learning patterns in sequential data (like text, speech).
    - Key for NLP tasks like translation, summarization, etc.

11. **Why Recurrence is Necessary**:
    - Sequences have dependencies on prior elements; RNNs can retain information from earlier words in a sentence to inform later ones.
    
12. **Backpropagation Through Time (BPTT)**:
    - A variant of backpropagation for RNNs, where errors are propagated through each time step in the sequence.
    - Major challenge: Vanishing/exploding gradients.

13. **Understanding Gates in RNNs**:
    - Gates control the flow of information in advanced RNNs like LSTMs (Long Short-Term Memory) and GRUs (Gated Recurrent Units).
    - Types of gates: input gate, forget gate, output gate.

14. **RNN Basics and Challenges**:
    - RNNs process sequences by looping over each time step.
    - **Challenges**:
      - Vanishing gradients: Makes it hard to retain information over long sequences.
      - Exploding gradients: Causes instability in training.

---
