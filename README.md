# Quantum Machine Learning for Conspicuity Detection in Production

## Project Overview

This project aims to optimize the production process by detecting deviations and weak points through conspicuity detection. By analyzing process data such as image data or time series, we identify areas for improvement within production workflows. Traditional analysis methods are often time-consuming, so this project explores the potential of hybrid quantum computing to accelerate these processes. Our primary goal is to implement hybrid quantum algorithms and benchmark them rigorously against classical approaches, including machine learning and statistical methods.

## Why This Project is Useful

Detecting anomalies and weak points in production processes at an early stage can significantly enhance efficiency and reduce costs. Hybrid quantum computing has the potential to process and analyze large datasets much faster than classical methods, enabling quicker identification and resolution of issues. This, in turn, improves overall productivity and quality in production environments.

## Getting Started

### Step 1: Familiarize Yourself with PennyLane and JAX

Before diving into the project, it's essential to understand the tools and frameworks we'll be using:

- **PennyLane**: A library for quantum machine learning, quantum computing, and quantum chemistry.
- **JAX**: A library for high-performance machine learning research.

**Action Items:**

1. Review the documentation and tutorial materials for PennyLane and JAX.
2. Implement and present the PennyLane x JAX tutorial to gain practical experience.

### Step 2: Implementing Quantum Neural Networks (QNNs)

In this step, you will develop Quantum Neural Networks (QNNs) with various scaling approaches:

1. Develop QNN prototypes using PennyLane and JAX.
2. Present the results using standard metrics (accuracy, precision, recall, F1-score) and visualization techniques.

### Step 3: Benchmarking Against Classical Methods

After implementing QNNs, the next step is to compare their performance against classical machine learning and statistical methods:

1. Benchmark the hybrid quantum algorithms against classical methods.
2. Visualize and compare the performance metrics.

## Dataset

For this project, we used three datasets across different tasks:

- **Detecting Anomalies in Wafer Production**: This dataset is particularly relevant to the semiconductor industry, where improvements in wafer production processes are critical.
- **MNIST Dataset**: We also used the MNIST dataset, a well-known benchmark in machine learning, to validate our model's learning capability. The model demonstrated good learning performance on the MNIST dataset, confirming its effectiveness.
- **TIG Alüminyum 5083 Dataset (Task 5)**: For Task 5, we utilized the TIG (Tungsten Inert Gas) Alüminyum 5083 dataset. This dataset is critical for analyzing the welding process of the Alüminyum 5083 alloy, commonly used in marine and industrial applications due to its excellent corrosion resistance and high strength. By applying quantum machine learning models, we aimed to detect defects and anomalies in the welding process, improving the quality control of production.

### TIG Alüminyum 5083 Dataset (Task 5)

This dataset contains detailed information about the welding parameters, temperature readings, and structural integrity of the Alüminyum 5083 alloy during the TIG welding process. The data is crucial for understanding and optimizing welding parameters to ensure high-quality welds, minimizing defects such as cracks and porosity. The integration of quantum machine learning models aimed to enhance the detection of these defects by analyzing the complex relationships between the variables in the dataset.

## Reducing the Size of the Training Dataset

To manage the dataset size and speed up the training process, we reduced the number of images per class. This was achieved by downsampling the majority classes to create a more balanced dataset, which is crucial for avoiding model bias towards more frequent classes.

## Splitting the Dataset into Training and Validation Sets

We split the reduced dataset into training and validation sets using an 80-20 split. This step ensures the model is trained and validated on independent sets of data, providing a more accurate assessment of its performance.

## Preparing Data for Model Training

Data preprocessing involved setting up image transformations using `torchvision`. These transformations include center cropping, converting images to tensors, and normalizing them, which helps standardize the input data and facilitates effective model learning.

## Defining the Quantum Circuit

A key component of the project is the definition of the quantum circuit, implemented using the Pennylane library. The quantum node (qnode) is created with angle embeddings and basic entangler layers, which process the input data and return Pauli-Z measurements. This circuit is then integrated with PyTorch, enabling a hybrid quantum-classical machine learning approach.

## Constructing the Hybrid Quantum-Classical Model

The hybrid model combines classical convolutional layers with a quantum layer. The classical layers process image data, and the quantum layer applies quantum computations to the processed data. Finally, fully connected layers perform classification based on the quantum layer’s output.

## Evaluating Model Performance

After training, the model's performance is evaluated on the validation set. This assessment provides insight into the model's ability to generalize to new data, and helps identify areas for improvement.

### MNIST Performance:
- The model demonstrated good learning on the MNIST dataset, achieving high accuracy and strong performance metrics across all evaluation criteria.

### Wafer Production Performance:
- The results were promising, though further tuning and optimization are required to fully harness the quantum approach's potential.

### TIG Alüminyum 5083 Performance (Task 5):
- The application of the model to the TIG Alüminyum 5083 dataset showed potential in identifying welding defects. The quantum-classical hybrid model was particularly effective in recognizing subtle patterns in the data that are critical for ensuring the structural integrity of welded components.

## Visualizing Training Accuracy

The training accuracy is visualized by plotting accuracy over epochs, which helps analyze the model’s learning curve and the effectiveness of the training process.

## Conclusion

In tackling class imbalance, we reduced the dataset by downsampling the majority classes, ensuring a balanced dataset to prevent bias in model predictions. Although accuracy was used as a validation metric, we remained aware of its limitations, especially in the context of class imbalance. Alternative approaches such as k-fold cross-validation and stratified splitting were considered, but a simpler split was chosen due to time constraints. Throughout the project, we were vigilant in monitoring for overfitting and underfitting, and made careful decisions about model complexity to balance these concerns.

The quantum aspect of the project relied heavily on the concept of an ansatz—a parameterized quantum circuit within the hybrid model. The choice of ansatz was critical, as it influenced the model's ability to capture complex patterns in the data.

## Getting Help

For assistance with the project, refer to the documentation and tutorials for PennyLane and JAX. You can also contact the project maintainers:

- **Betül Gül** (eng.betulgul@gmail.com)

## Maintainers and Contributors

- **Betül Gül** - Womanium Program Enrollment ID: WQ24-zlmRFieHjeFCWok

## Presentation Slides

You can view our presentation slides [here](https://www.canva.com/design/DAGNT_Nw_Qs/qKLHoUsYONmbQjA5onXAHQ/view?utm_content=DAGNT_Nw_Qs&utm_campaign=designshare&utm_medium=link&utm_source=editor).

