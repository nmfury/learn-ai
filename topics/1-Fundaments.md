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
  - This type of data is _suitable_ for **traditional machine learning algorithms** that **require** well-defined [features](#features) and [labels](#labels).
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

---

<a id="features"></a>
**Features**

<a id="labels"></a>
**Labels**
