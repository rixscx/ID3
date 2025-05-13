# 🌳 ID3 Algorithm (Iterative Dichotomiser 3)

**Purpose:**  
The ID3 algorithm is used to build a **decision tree** for **classification** tasks by recursively selecting the feature that offers the highest **information gain**.

---

## 📌 Key Concepts

### 1. Entropy (H)
A measure of uncertainty or impurity in a dataset.  
Formula for a binary classification:

H(S) = -p₊ log₂(p₊) - p₋ log₂(p₋)


Where:
- `p₊`: Proportion of positive examples  
- `p₋`: Proportion of negative examples

---

### 2. Information Gain (IG)
The reduction in entropy achieved by splitting the dataset on an attribute.

IG(S, A) = H(S) - ∑ [ (|Sv| / |S|) * H(Sv) ]


Where:
- `S`: The full dataset  
- `A`: The attribute  
- `Sv`: Subset of S where attribute A has value v  

---

## 🧠 ID3 Algorithm Steps

1. **Start** with the entire dataset.
2. **Calculate entropy** for the dataset.
3. **For each attribute**, calculate **information gain**.
4. **Select the attribute** with the highest information gain as the decision node.
5. **Split** the dataset based on that attribute.
6. **Repeat** the process recursively for each child node until:
   - All instances in a node belong to the same class, or
   - There are no more attributes to split on

---

## ✅ Advantages

- Simple and easy to implement  
- Works well with categorical data

---

## ❌ Limitations

- Can overfit on noisy data  
- Biased towards attributes with more levels  
- Doesn’t handle numeric attributes natively (ID3 assumes categorical)

---

## 📦 Example (Simplified)

**Dataset:** Play Tennis  
**Attributes:** Outlook, Temperature, Humidity, Wind

**ID3 Process:**
- Calculate IG for each attribute
- Pick "Outlook" (highest IG) as the root
- Split on Outlook: Sunny, Overcast, Rain
- Recursively build branches for each value

---

## 🔁 Related Algorithms

- **C4.5**: Successor to ID3, handles continuous attributes and pruning  
- **CART**: Builds binary trees using Gini Index or entropy

---

## 🙋‍♀️ Contributing

Pull requests are welcome! You can contribute by adding:

- 📈 Visualizations  
- 📓 Notebooks for classification/regression use cases  
- 📊 Sample datasets  
- 🔁 ID3 implementations in different languages  

---

## 📬 Contact

Questions or feedback? Reach out via [LinkedIn](https://www.linkedin.com/in/rixscx) or open an issue on this repository.



### 🙌 **Contributors**
#### [Manish P](https://github.com/rixscx) <br>
#### under guidance of [Dr Agughasi Victor Ikechukwu](https://github.com/Victor-Ikechukwu) <br>
---

❤️ Thank You!
Thank you for checking out our project! We hope this inspires you to explore the intersection of AI and healthcare. Feel free to reach out for questions, suggestions, or collaborations.

<br><br>
