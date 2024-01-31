Comparing Quantum Neural Network with Single-layer MLP for Stock Price Time Series Forecasting using Qiskit and Quantum Computing Theory
1. Overview of Stock Price Prediction with Quantum Machine Learning:
- It explores the comparison of a quantum neural network with a simple single-layer MLP for stock price time series forecasting.
- Historical stock data from Financial Modeling Prep's API is used for the analysis.
2. Importing and Setting up Environment:
- The necessary libraries including Qiskit, numpy, pandas, and tensorflow are imported for the analysis.
- The Qiskit library is installed to work with quantum computing networks.
3. Introduction to Quantum Computing:
- Quantum computers use qubits which can be both 0 and 1 at the same time, unlike traditional bits.
- Quantum gates work with qubits and exhibit unique behaviors like superposition and entanglement.
4. Operators in Quantum Computing:
- Quantum gates perform operations using complex numbers and Matrix operations.
- The Controlled-NOT (CNOT) gate creates entanglement between qubits, enabling coordinated behavior.
5. Parameterized Gates and Quantum Circuits:
- Rotation gates like R_x(θ), R_y(θ), and R_z(θ) allow customizable quantum algorithms.
- Quantum circuits represent quantum algorithms and incorporate parameterized gates for flexibility.
6. Quantum Machine Learning (QML):
- QML utilizes quantum operations and features like superposition and entanglement for conventional machine learning tasks.
- The Quantum Neural Network (QNN) in QML resembles a classical neural network but operates with qubits and parameterized gates.
7. Significance of Parameterized Gates in QML:
- Parameterized gates introduce a customizable element into quantum algorithms by adjusting input parameters.
- The flexibility of this approach optimizes and customizes the performance of quantum algorithms for specific tasks.
8. Design and Creation of QML Model:
- A QML model typically involves the creation of a Variational Quantum Circuit (VQC) with parameterized gates.
- The QNN incorporates entanglements and mechanisms for information exchange among qubits.
9. Quantum Neural Network:
- The quantum neural network consists of three main layers: Input Layer, Ansatz Layer, and Output Layer.
- The input layer transforms classical input data into a quantum state using a parameterized variational circuit, while the ansatz layer contains a Variational Quantum Circuit and the output layer performs measurements on qubits.
10. Input Layer:
- The input layer employs a tensor product encoding technique, and it uses a simple X-rotation gate for each qubit, with learnable parameters for scaling and bias in the input data to enhance flexibility.
11. Ansatz Layer:
- The Real Amplitudes ansatz is adopted, initiating with full rotation X/Y/Z parameterized gates, followed by a series of CNOT gates arranged in a ring structure to facilitate qubit information transfer.
12. Output Layer:
- The network output is determined by calculating the expectation of the σ_z operator over the quantum state, with the result falling within the range of [-1, 1].
- A final scale parameter and bias to be learned are introduced to make the network output less sensitive to biases and scales inherent in the dataset.
13. Model Training:
- The training of the proposed Quantum Neural Network happens on a regular CPU using classical algorithms like the Adam optimizer, while the Quantum Processing Unit (QPU) is used for specific quantum computations.
14. Time Series Forecasting:
- For time series forecasting with Quantum Neural Network, the temporal variable is transformed into a tabular format, and the inputs encompass the values at different time points to facilitate the model’s understanding of temporal relationships for making predictions.
- Data preprocessing and feature mapping are carried out to encode data into qubits and optimize the model using the Pauli Feature Map and ADAM optimizer.
15. Coding and Data Preprocessing:
- The data is fetched using the historical Data API endpoint provided by Financial Modeling Prep, and the open price is selected as the temporal variable for further processing.
- The acquired data is preprocessed and input-output data is created for time series forecasting using the Pauli Feature Map and ADAM optimizer for encoding and optimizing the model.
16. Quantum Circuit:
- The quantum circuit function initializes a quantum circuit with a specified number of qubits and depth, incorporating parameterized gates for quantum information transfer and facilitating qubit operations.
17. Quantum Neural Network Ansatz:
- The ansatz circuit is constructed by appending rotation gates with parameterized rotational angles in the first loop and adding CNOT gates in the second loop, effectively creating the quantum neural network structure.
- This process constructs the ansatz for the quantum circuit, defining the quantum neural network structure.
18. VQC Integration and Fitting:
- A Variational Quantum Circuit (VQC) is created by incorporating the ansatz and the encoding for features, simplifying the implementation of quantum machine learning algorithms.
- The VQC is fitted to the features and its performance is assessed, demonstrating its effectiveness in handling the given features and predicting outcomes.
19. Classical Neural Network:
- A Multilayer Perceptron (MLP) classical neural network with a single hidden layer and 64 nodes is constructed for comparison with the quantum neural network.
- The classical neural network serves as a benchmark for evaluating the performance of the quantum neural network.
20. Result and Comparison:
- The Quantum Neural Network (QNN) outperforms the Artificial Neural Network (ANN) with a Root Mean Squared Error (RMSE) of less than 3.5, indicating its promising potential.
- Quantum Neural Networks (QNN) hold promise for further development and practical implementation, showcasing their potential for time series forecasting.
21. Conclusion:
- The experiment highlights the potential of quantum computing and neural networks for future growth, indicating the promising path for the future of quantum computing in machine learning applications.
- Quantum machine learning algorithms have the potential to significantly reduce training times and enhance computational power, showcasing their impact on the future of machine learning.


References - https://medium.datadriveninvestor.com/stock-price-prediction-with-quantum-machine-learning-in-python-54948a3da389
           - https://chat.openai.com/share/b7a493dd-231d-4df0-918a-24148c598080
