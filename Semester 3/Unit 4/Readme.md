> The various topics inside unit 3 has been sorted into 3 categories. 
---

### **LSTM (Long Short-Term Memory) Networks**

1. **LSTM Basics**:
   - LSTMs are a type of RNN designed to handle long-term dependencies and mitigate issues like vanishing gradients.
   - They include memory cells that retain important information over long sequences.

2. **LSTM Structures**:
   - LSTMs use **gates** to control information flow:
     - **Input Gate**: Decides which information is added to the cell state.
     - **Forget Gate**: Chooses which information to discard.
     - **Output Gate**: Determines the next hidden state.
   
3. **Applications of LSTM**:
   - Used widely in time-series prediction, language modeling, machine translation, and speech recognition.

4. **Sentiment Analysis**:
   - LSTMs can analyze sequences of text to determine sentiment by learning context across words or sentences.

5. **Machine Generation**:
   - LSTMs are used to generate text by learning sequential data patterns (e.g., predicting the next word based on previous ones).

6. **Adiayer LSTM Structures** (likely "Hierarchical" or "Advanced" LSTM Structures):
   - Variants like **Bidirectional LSTM** and **Stacked LSTM** improve performance for complex tasks by processing input in both forward and backward directions or stacking multiple LSTM layers.

---

### **Advanced Language Models and Architectures**

7. **Advanced Language Models**:
   - Include models trained on large datasets for tasks like translation, summarization, and question answering.
   - Models: GPT, BERT, XLNet (discussed below).

8. **Bidirectional LSTM**:
   - Processes data in both forward and backward directions to capture context from both ends of a sequence.
   - Useful for tasks where understanding the full context is essential, such as entity recognition.

9. **Attention Mechanism**:
   - Helps models focus on specific parts of a sequence, assigning "attention weights" to relevant words.
   - Improves performance in sequence-to-sequence tasks like translation.

10. **Challenges in LSTM**:
    - Still prone to vanishing gradients with very long sequences.
    - Computationally intensive for large datasets or long texts.

---

### **Transformers and Modern Architectures**

11. **Encoder-Decoder Architecture**:
    - Common in sequence-to-sequence tasks (e.g., machine translation).
    - The encoder processes the input sequence into a fixed representation, which the decoder then uses to generate the output.

12. **Transformers**:
    - A neural network architecture that relies on **attention mechanisms** instead of recurrence.
    - More efficient than LSTMs for parallel processing of sequence data.
   
13. **BERT (Bidirectional Encoder Representations from Transformers)**:
    - A pre-trained Transformer model that reads text in both directions, capturing full context for each word.
    - Performs well on various NLP tasks after fine-tuning.

14. **XLNet**:
    - An extension of BERT that addresses BERT's limitations by using a permutation-based training objective.
    - Achieves better performance on tasks by capturing more varied contexts.

---
