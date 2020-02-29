# Machine learning for quantum states learning

#### In this repo you will find 2 Jupyter notebooks:
* The first one uses pennylane framework only for its simplicity and to prepare the reader for the second notebook. It also serves as a proof of concept notebook for machine learning purposes.
* The second notebook demonstrates the usage of Qiskit and some of its important modules to perform the required task. It also includes two different ways for learning through its Aqua modules or by a user defined gradient and cost functions.

### Ans for Q1 and Bouns Q:

Best architecture is a single <a href="https://www.codecogs.com/eqnedit.php?latex=R_y" target="_blank"><img src="https://latex.codecogs.com/gif.latex?R_y" title="R_y" /></a> gate and a CNOT gate. I have also included a working example showing why would the <a href="https://www.codecogs.com/eqnedit.php?latex=R_y" target="_blank"><img src="https://latex.codecogs.com/gif.latex?R_y" title="R_y" /></a> gate would be the best option. It's also good to include the statevector fidelity to ensure that the final state is the required one.

### Ans for the stochastic nature of the measurements:

* In pennylane's notebook and also Qiskit's one, the **100** shots trial was the best one in terms of stability and speed of convergence. The same result is confirmed in the following [paper](https://arxiv.org/pdf/1910.01155.pdf).
* Another **important note**, in qiskit's notebook I had to set the optimization level to the maximum so that the transpiled circuit would be the perfect match for Vigo's architecture.
* Initializing the weights between 0 and 1 avoids negative values for rotation gate but taking the abs value will ensure that it's going to give us the required positive state



