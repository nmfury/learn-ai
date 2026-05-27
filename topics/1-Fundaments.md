# Fundamentals

You are here: topics/1-Fundamenta.md | [🏠︎](../README.md)

---

## Basics

Artificial Intelligence (AI) is an **umbrella term** and is a broad field that encompasses the research and development of intelligent systems.
These intelligent systems are capable of performing tasks that typically require human intelligence, such as _perception_, _reasoning_, _learning_, _problem-solving_, and _decision-making_.

```code
-----------------------------------
|    Artificial Intelligence
|    ------------------------------
|    |    Machine Learning
|    |    -------------------------
|    |    |   Deep Learning
|    |    |   ---------------------
|    |    |   |    Generative AI
-----------------------------------
```

- **Machine Learning (ML)**: a subset of AI, is a field in computer science that is heavily focused on building methods that make it possible for machines to learn.
- **Deep Learning (DL)**: a subset of ML, maps the concepts of _neurons_ and _synapses_ - a topic from the world of human anatomy, to build systems that are able to rely information from one neuron to other.
- **Generative AI**: A subset of deep learning. These systems are capable of **generating new data** based on the **patterns** and **structures** learned from _training data_. They can adapt models built using deep learning but _without retraining_ or _fine tuning_.

## Machine Learning Fundamentals

**Data collection** is the _fundamental step_ towards building machine learning models. A **machine learning model** is a program that learns patterns from the data so that it is can make predictions / decisions on new data.

**In simpler terms:**

- An **Algorithm**, is the method used to learn from data
- The **Training**, is the process of feeding data to that algorithm
- The **Model**, is the final learned system that can make predictions

Example:

- **Task**: predict house prices
- **Data**: size, location, number of rooms, and actual prices
- **Algorithm**: linear regression
- **Training**: the algorithm looks at many examples and finds relationships
- **Model**: the learned formula that can estimate the price of a new house

### The Training Data

The main types of data used in training are _structured_ and _unstructured_ data.

- **Structured data:**
  - Data that is _organized_ and well _formatted_, typically in the form of _tables_ or _databases_ with **rows** and **columns**.
  - This type of data is _suitable_ for **traditional machine learning algorithms** that **require** well-defined [features and labels](#features-and-lables).
  - The following are types of structured data.
    - **Tabular data**: Data stored in spreadsheets, databases, or CSV files, with rows representing instances and columns representing features or attributes.
    - **Time-series data**: Data consists of sequences of values measured at _successive points_ in time, such as _stock prices_, _sensor readings_, or _weather data_.
- **Unstructured data:**
  - Data that lacks a predefined structure or format.
    - **Text data:** This includes documents, articles, social media posts, and other textual data.
    - **Image data:** This includes digital images, photographs, and video frames.
  - With unstructured data, we have the following two categories of data:
    - **Labeled data:** is a dataset where each `data point` or `example` is has a label. In other terms, the _target variable_ represents the **desired** _output_ or _classification_.
      - These labels are typically provided by human experts or obtained through a reliable process.
      - **Example:** In an image classification task, labeled data would consist of images along with their corresponding class labels (for example, cat, dog, car).
    - **Unlabeled data**: is a dataset where the instances or examples **do not have** any associated labels or target variables.
      - The data consists only of input features, without any corresponding output or classification.
      - **Example**: A collection of images without any labels or annotations.

### Machine Learning Process

After the ETL (extract-transform-load) step, a subset of data is compiled into a **training set** - that data on which the learning happens.

- In **supervised learning**, the algorithms are _trained_ on _labeled data_. The goal is to **learn** a **mapping function** that can **predict** the output for new, unseen input data.
- **Unsupervised learning** refers to algorithms that **learn** _from_ **unlabeled data**. The **goal** is to _discover_ **inherent patterns**, **structures**, or **relationships** within the input data.
- In **reinforcement learning**, the machine is fed with a _portion_ of labeled training data. A **performance score** is given to the machine as **guidance** - it is form of **semi-supervised learning**. The **feedback** is _provided_ in the form of **rewards** or **penalties** for its _actions_, and the machine learns from this feedback to improve its decision-making over time.

**Inferencing** is the next step in the process. A model is now fed **test data** to validate the learnings, its ability to make predictions and/or decisions.

- **Batch inferencing** is when the machine takes a large amount of data, such as images or text, and analyzes it all at once to provide a set of results.
  - This type of inferencing is often used for tasks like data analysis, where the speed of the decision-making process is not as crucial as the accuracy of the results.
- **Real-time inferencing** is when the computer has to make decisions quickly, in response to new information as it comes in.
  - This is important for applications where immediate decision-making is critical, such as in _chatbots_ or _self-driving cars_.

<br>

---

<br>

## Deep Learning Fundamentals

The field of **deep learning** is inspired by the **structure** and **function** of the **_brain_**. It involves the _use_ of **artificial neural networks**, which are computational models that are designed to _mimic_ the way the **_human brain_** processes information.

### Neural Networks

Neural networks mimic our brains. The _neurons_ that are connected to each other, map to tiny units called **nodes**, that are connected together.

These nodes are **organized** into **layers**. The layers include an **input layer**, **one or more hidden layers**, and **an output layer**.

**How information is passed:**

- The **input layer** receives the _features_. For example, a typical set of features that a customer can have are - _age_, _purchase history_, or _app usage_.
- This information is sent to the **hidden layers**.
- **Each connection** has a **weight** marking its _importance_.
- Each node _combines_ the inputs it receives, performs a action - calculation, and passes the result forward.
- Finally, the **output layer** gives the _prediction_, like "likely to buy" or "unlikely to buy".

**During training, one more step happens:**

- The **network** _checks_ the accuracy of its prediction, determining the closeness to the real answer.
- Then it **adjusts** the **weights** in the **connections**.
- This helps it make better predictions next time.

**Computer Vision** a field of artificial intelligence that makes it possible for computers to interpret and understand digital images and videos. Deep learning has provided powerful techniques for achieving tasks such as _image classification_, _object detection_, and _image segmentation_.

**Natural Language Processing** a branch of artificial intelligence that deals with the interaction between computers and human languages. Deep learning has enabled achievement of tasks such as _text classification_, _sentiment analysis_, _machine translation_, and _language generation_.

<br>

---

<br>

### References

<a id="features-and-lables"></a>
**Features and Labels**

- **Features** are the input information the model uses to learn.
- **Labels** are the correct answers it’s trying to predict.

| Size (sq ft) | Bedrooms | Location Score | Price  |
| ------------ | -------- | -------------- | ------ |
| 1200         | 2        | 7              | 200000 |
| 1800         | 3        | 8              | 320000 |
| 2500         | 4        | 9              | 500000 |

In this example:

- features: `Size`, `Bedrooms`, `Location Score`
- label: `Price`

So the model looks at the **features** and _learns_ to **predict** the **label**.
