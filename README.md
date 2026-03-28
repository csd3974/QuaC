# QuaC

## 📁 Notebooks Overview

### 1. QuaC.ipynb
In this notebook we guide you through how the QuaC idea works and allow you to visualize each step of the algorithm. Finally you can run your own tests classically and through the Aer Simulator of Qiskit.

### 2. Grover_vs_QuaC.ipynb
In this notebook, we run some simple tests to compare the performance of Grover's Alrogithm against QuaC. You are able to edit the marked states of Grover by editing the corresponding cell. Then run the cells sequentially and observe the results.

### 3. QuaC_measuring.ipynb
In this notebook, we are extending our tests by including real Quantum Hardware through IBM's open plan. We also compare Grover once again with the difference of hardware noise being included as a variable due to the real Quantum hardware.

### 4. QuaC_on_real_datasets_paper.ipynb
In this notebook, we run experiments to observe the performance of QuaC on real datasets. The input dataset has to be in the form of a csv. You can test your own datasets by editing 
```bash
'with open('dataset_name.csv', mode ='r')as file:'
```
in the second and third cell of the code.

---

## ⚙️ Installation

1. Clone the repository:

```bash
git clone https://github.com/csd3974/QuaC.git
cd QuaC
```
2. (Optional but recommended) Install Conda and create a virtual environment:
https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html

```bash
conda create --name <my-env>
conda activate <my-env>
```

3. Install dependencies:

```bash
pip install qiskit
pip install qiskit-aer
pip install qiskit-ibm-runtime
pip install matplotlib
```

## Running on IBM

In order to run experiments on real Quantum hardware by IBM you will need to create an account on IBM (https://quantum.cloud.ibm.com) and get your free API token. Then you need to paste your token in QuaC_measuring.ipynb and specifically in this line
```bash
token="", #Insert your API key here
```
After that, you can either pick a specific Quantum computer to run the experiments on or by default our code will select the least busy one. 

## Getting Started

After you have completed the Installation steps above and have gotten your IBM token (if you want to run real hardware experiments) the only thing left to do is navigate through the .ipynb files, run the cells sequentially and observe the experiment results.

