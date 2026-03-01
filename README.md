# machine-learning-project-Detecting Spam Emails Using Tensorflow in Python



## 📌 1️⃣ Basic Libraries

```python
import numpy as np
```

👉 **NumPy**
Used for:

* Mathematical operations
* Working with arrays (vectors, matrices)
* Fast numerical computation

`np` is just a short name (alias).

---

```python
import pandas as pd
```

👉 **Pandas**
Used for:

* Reading CSV files
* Handling datasets
* Data cleaning & manipulation

`pd` is alias.

---

```python
import matplotlib.pyplot as plt
```

👉 **Matplotlib**
Used for:

* Plotting graphs
* Data visualization

`plt` is commonly used alias.

---

```python
import seaborn as sns
```

👉 **Seaborn**

* Advanced visualization library
* Built on top of Matplotlib
* Makes graphs more beautiful and statistical

`sns` is alias.

---

## 📌 2️⃣ Text Processing Libraries (NLP)

```python
import string
```

👉 Python built-in module
Used for:

* Accessing punctuation
* String constants (like ascii letters)

Example:

```python
string.punctuation
```

---

```python
import nltk
```

👉 **Natural Language Toolkit (NLTK)**
Used for:

* Text preprocessing
* Tokenization
* Stopword removal
* Stemming / Lemmatization

---

```python
from nltk.corpus import stopwords
```

👉 Importing **stopwords list**

Stopwords = common words like:

* is
* the
* and
* in
* of

We remove them because they don't carry much meaning.

---

```python
from wordcloud import WordCloud
```

👉 Used to generate **word cloud visualization**

Word cloud = words displayed based on frequency
More frequent → Bigger size

---

```python
nltk.download('stopwords')
```

👉 Downloads stopwords dataset from NLTK
This runs once and stores locally.

---

## 📌 3️⃣ Deep Learning (TensorFlow & Keras)

```python
import tensorflow as tf
```

👉 **TensorFlow**

* Deep learning framework
* Used for building neural networks

---

```python
from tensorflow.keras.preprocessing.text import Tokenizer
```

👉 **Tokenizer**
Used for:

* Converting text → numbers
* Assigning index to words

Example:

```
"I love AI"
→ [1, 5, 10]
```

---

```python
from tensorflow.keras.preprocessing.sequence import pad_sequences
```

👉 Used for:

* Making all text sequences same length
* Adds zeros if needed

Example:

```
[1, 5]
[1, 5, 10, 7]

→ padded
[0,0,1,5]
[1,5,10,7]
```

Neural networks require equal length inputs.

---

```python
from sklearn.model_selection import train_test_split
```

👉 From **Scikit-Learn**

Used to:

* Split dataset into

  * Training set
  * Testing set

Example:

```
80% training
20% testing
```

---

```python
from keras.callbacks import EarlyStopping, ReduceLROnPlateau
```

### 🔹 EarlyStopping

Stops training automatically when:

* Model stops improving
* Prevents overfitting

### 🔹 ReduceLROnPlateau

Reduces learning rate when:

* Model performance stops improving
* Helps better convergence

---

## 📌 4️⃣ Warnings Handling

```python
import warnings
```

👉 Built-in module to handle warnings.

---

```python
warnings.filterwarnings('ignore')
```

👉 Hides warning messages from output.
Keeps notebook clean.

---

# 🎯 Overall Meaning

This setup is typically used for:

✔ Text preprocessing
✔ Word cleaning
✔ Visualization
✔ Converting text to numeric format
✔ Training deep learning model
✔ Preventing overfitting
✔ Plotting results



