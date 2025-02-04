### **Shakespearean Text Generator**  

#### **Overview**  
This project implements an **n-gram language model** to generate text in the style of Shakespeare. It processes an input text file, builds n-gram frequency distributions, and generates new text based on learned probabilities.  

---

#### **Features**  
- **Text Preprocessing:** Converts input text to lowercase, removes punctuation, and tokenizes words.  
- **N-Gram Model:** Supports bigrams, trigrams, and quadgrams for text generation.  
- **Probability Computation:** Calculates token probabilities based on training data.  
- **Randomized Text Generation:** Uses weighted random sampling to generate text sequences.  
- **Backoff Strategy:** Attempts smaller n-grams when a match is not found.  

---

#### **Requirements**  
- Python 3.x  
- No external dependencies (uses built-in Python libraries)  

---

#### **Usage**  

1. **Prepare Input Text**  
   - Place a `.txt` file (e.g., `shakespeare.txt`) in your working directory.  

2. **Run the Script**  
   ```bash
   python nlp_module1.py
   ```

3. **Expected Output**  
   - The script will generate text based on the input file using different n-gram models:  
     ```
     Bigram Generated Text:
     to be or not to be that is the question...
     
     Trigram Generated Text:
     all the world’s a stage and all the men...
     
     Quadgram Generated Text:
     to be or not to be that is the question...
     ```

---

#### **File Structure**  
```
/project-directory
│── nlp_module1.py         # Main script for text generation
│── shakespeare.txt         # Input text file
│── README.md               # Project documentation
```

---

#### **Customization**  
- Modify `n` in the `build_ngram_counts()` function to experiment with different n-gram sizes.  
- Adjust `num_tokens` in `generate_text()` to control the length of generated output.  

---

#### **Limitations**  
- The model relies on probabilities from the input text and may repeat phrases.  
- Larger n-gram sizes require a more extensive corpus to generate meaningful text.  

---

#### **Future Improvements**  
- Implement **smoothing techniques** to handle unseen n-grams.  
- Enhance the **backoff strategy** for better text flow.  
- Allow **user input** to define the initial context for generation.  

---

This project demonstrates the basics of **n-gram-based text generation** and can be expanded further with **deep learning models** like LSTMs or transformers.

