
## Unit 3

### 1. **Basic HTML Tags, Beautiful Soup & Python Code for Web Scraping**

- **Basic HTML Tags**:
  - `<html>`: Root of an HTML document.
  - `<head>`: Contains metadata like `<title>`, `<meta>`, `<link>`.
  - `<title>`: Title of the web page displayed in the browser tab.
  - `<body>`: Main content of the HTML document.
  - `<h1>`, `<h2>`, etc.: Header tags for organizing content hierarchically.
  - `<p>`: Paragraph tag for text blocks.
  - `<a>`: Hyperlink tag for linking to other pages or resources.
  - `<img>`: Embeds images in a webpage.

- **Beautiful Soup**:
  - A Python library used to scrape data from HTML or XML documents. It parses HTML, allowing easy data extraction from websites.
  - **Features**:
    - Simple parsing and navigation of HTML/XML data.
    - Supports searching elements by tags, attributes, and CSS selectors.
    - Integrates well with `requests` for retrieving HTML content.
  
- **Python Code for Web Scraping**:
  ```python
  from bs4 import BeautifulSoup
  import requests

  url = "https://example.com"
  response = requests.get(url)
  soup = BeautifulSoup(response.text, 'html.parser')

  # Extract all links
  for link in soup.find_all('a'):
      print(link.get('href'))
  ```

---

### 2. **Bi-gram Model for Prediction**

To predict the word that follows “I really”:

- **Corpus**:
  - S1: I really appreciate your help.
  - S2: I am really sorry for not inviting you.
  - S3: I really appreciate your hard work.
  - S4: I really like your watch.

- **Bi-gram Model**:
  - A bi-gram model uses pairs of words to predict the next word. The context “I really” pairs with “appreciate” (twice), “sorry,” and “like.”
  
- **Prediction**:
  - The bi-gram with “I really” has the following words:
    - “appreciate” (frequency: 2)
    - “sorry” (frequency: 1)
    - “like” (frequency: 1)
  - Based on frequency, **“appreciate”** is the most likely prediction.

---

### 3. **Types of LSTM and Applications**

- **Vanilla LSTM**: Basic LSTM with a single input and output. Used for standard sequence prediction tasks like **sentiment analysis**.
- **Bidirectional LSTM**: Processes input in both forward and backward directions. Useful in **speech recognition**.
- **Stacked LSTM**: Multiple LSTM layers stacked to capture more complex patterns. Applied in **language translation**.
- **CNN-LSTM**: Combines CNNs for spatial feature extraction with LSTMs for sequence learning. Used in **video analysis**.

---

### 4. **XLNet Architecture**

- **XLNet Overview**:
  - Uses a permutation-based training approach, generating sequences in a flexible order rather than left-to-right.
  - Combines **bidirectional context** modeling with **autoregressive prediction**, improving on BERT for certain NLP tasks.

- **Working Example**:
  - Suppose we want to predict the next word in “The weather is ___.”
  - XLNet permutates the input sequence in various ways (like “is the weather”) and learns bidirectional dependencies.

- **Illustrative Code**:
  ```python
  from transformers import XLNetTokenizer, XLNetForSequenceClassification
  import torch

  tokenizer = XLNetTokenizer.from_pretrained("xlnet-base-cased")
  model = XLNetForSequenceClassification.from_pretrained("xlnet-base-cased")

  inputs = tokenizer("The weather is", return_tensors="pt")
  outputs = model(**inputs)
  ```

---

### 5. **Scraping E-commerce Sites with BeautifulSoup**

To build a price comparison tool:

- **Steps**:
  1. **Identify Target Elements**: Find the HTML structure of product prices and specifications.
  2. **Scrape Data**: Use BeautifulSoup to retrieve details.
  3. **Store and Compare**: Store prices from multiple sources in a database, and run comparisons.
  
- **Example Code**:
  ```python
  from bs4 import BeautifulSoup
  import requests

  url = "https://ecommerce-site.com/product"
  response = requests.get(url)
  soup = BeautifulSoup(response.text, 'html.parser')

  # Extracting price
  price = soup.find('span', class_='product-price').text
  specs = soup.find('ul', class_='product-specs').text

  print("Price:", price)
  print("Specifications:", specs)
  ```

---

### 6. **N-gram Model**

- **N-gram Model**:
  - Uses a sequence of N words to predict the next word in a sentence. Commonly used N-grams include bigrams (2 words) and trigrams (3 words).
  
- **Example**:
  - For the sentence “I am learning NLP,” possible bigrams include “I am,” “am learning,” “learning NLP.”

---

### 7. **LSTM-based POS Tagging**

Using an LSTM model for part-of-speech (POS) tagging:

- **Example**:
  - Sentence: “The cat sat on the mat with a hat.”
  - POS tags:
    - The: DET
    - cat: NOUN
    - sat: VERB
    - on: PREP
    - the: DET
    - mat: NOUN
    - with: PREP
    - a: DET
    - hat: NOUN

---

### 8. **Encoder-Decoder Model**

- **Working Principle**:
  - The **encoder** processes input data and encodes it into a fixed-size context vector.
  - The **decoder** then generates output by interpreting this context vector, making it ideal for tasks like **language translation**.
  
- **Applications**:
  - **Machine Translation**: Translating text from one language to another.
  - **Image Captioning**: Generating descriptions for images by using visual data as input to the encoder. 

- **Sketch**:
  ```
  Input Sequence --> Encoder --> Context Vector --> Decoder --> Output Sequence
  ```
