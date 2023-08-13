# Quantum-Programming-Algorithms-with-Qiskit
Quantum Programming Algorithms with Qiskit : This notebook presents algorithms and examples used in Quantum programming with Qiskit. It includes Teleportation, Bernstein Vazirani Algorithm, Deutsch Algorithm, Grover Algorithm.

Hadamard gate:

Superposition Creation: The Hadamard gate, when applied on a single qubit, creates a superposition state in which the qubit is in a combination of both states, rather than just in the 0 or 1 state. For example, applying a Hadamard gate yields a superposition state between state |0⟩ (classical 0) and state |1⟩ (classical 1): (|0⟩ + |1⟩) / √2.

Teleportation:

It involves manipulating quantum gates, measurements and quantum states used when building quantum circuits or quantum algorithms. The programming of quantum teleportation may include the following steps:

1. Quantum Circuit Design: The first step involves the design of the quantum circuit in which quantum teleportation will be performed. This circuit includes the steps by which quantum teleportation will take place by measuring the state of the source particle and adapting the state of the target particle.

2. Quantum Gates: Quantum gates, used in the creation of quantum circuits, are the basic processing units of quantum computers. Gates such as Hadamard, CNOT, Toffoli are used to manipulate quantum states.

3. Quantum States: Quantum programming uses mathematical expressions and libraries to represent and manipulate quantum states. These states represent the states of qubits and quantum systems.

4. Measurements: The quantum teleportation process is realised through measurements. Quantum programming involves setting up measurements accurately and using the measurement results.

   

Controlled-X (CX) Gate:

The CX gate is a very important gate in quantum computing and performs a controlled bit flip between two qubits. This gate is also called CNOT (Controlled NOT) gate.

The logic of the Controlled-X (CX) gate is as follows: It operates between two qubits, a control qubit and a target qubit. If the control qubit is 1 (or True), a bit flip (X gate) is applied on the target qubit. If the control qubit is 0 (or False), no operation is performed.

This gate is used in quantum circuits to perform many different computational and logical operations. It represents a general class of controlled gates and is used in various quantum algorithms.



Z Gate:

The expression circuit.z(0) is used to apply a Z gate to a given qubit in a quantum circuit. The Z gate is one of the fundamental gates used in quantum computing and corresponds to the Pauli Z matrix (z-matrix).

The Pauli Z matrix is defined as follows:

Z = | 1 0 | | 0 -1 |

This matrix multiplies state 0 by 1 and state 1 by -1, i.e. it returns a qubit only by applying a phase change. In other words, the Z gate changes the phase on a qubit.



X Gate:

The expression circuit.x(0) is used to apply an X gate to a given qubit in a quantum circuit. The X gate is one of the fundamental gates in quantum computing and corresponds to the Pauli X matrix (x-matrix).

The Pauli X matrix is defined as follows:

X = | 0 1 | | 1 0 | This matrix replaces state 0 with 1 and state 1 with 0. That is, it changes a qubit from state 0 to state 1 or from state 1 to state 0. This performs a "bit flip" operation on the qubit.

If you use circuit.x(0), an X gate is applied to the first (0 indexed) qubit in the specified quantum circuit and the state of the qubit changes.



Controlled-Z (CZ) Gate:

The CZ gate operates between two qubits and affects the phase state on a control qubit on the target qubit. If the control qubit is in state 1 (or True), the Z gate is applied on the target qubit and the phase state changes. If the control qubit is 0 (or False), no action is taken.

The matrix of the controlled Z gate is as follows:

CZ = | | 1 0 0 0 0 | | 0 1 0 0 | | 0 0 1 0 | | 0 0 0 -1 | The controlled-Z gate is used in quantum computing for various operations and gate combinations. In particular, the CZ gate can be used to change the entanglement state between two qubits.



Bernstein Vazirani Algorithm:

The Bernstein-Vazirani Algorithm is a quantum computing algorithm used by quantum computers to find a given sequence of hidden bits. While a classical computer requires linear time for such a string discovery, the Bernstein-Vazirani Algorithm performs this operation in constant time using quantum parallelisation.

This algorithm is particularly useful in a scenario where there is a "magic" function that gives the correct answer in a limited number of questions. The algorithm uses the results of a magic function to determine the secret input bit sequence of this magic function.

The logic of the Bernstein-Vazirani Algorithm consists of the following steps:

1. A qubit array is created. A superposition between all states is created by applying Hadamard gates on this array.
2. The magic function is applied to the qubits as a gate shaped according to the hidden bit sequence.
3. Finally, Hadamard gates are again applied to the qubits and the resulting qubit array is measured.
   
The algorithm is designed to determine the hidden bit sequence as a result of these steps. This algorithm takes advantage of quantum parallelisation to solve a problem that is complex for classical computers more quickly.



Deutsch Algorithm:

  The Deutsch Algorithm is a basic quantum computing algorithm used by quantum computers to determine whether a "magic" function that gives a correct   
  answer in a limited number of questions is stable or unstable. The algorithm requires two queries in the worst case to perform the same operation by a 
  classical computer, while the Deutsch Algorithm can detect this state with only one query.

  This algorithm works on two qubits and consists of the following steps:

  A qubit array is created and a superposition state is generated with Hadamard gates. The magic function is applied to the qubit as a gate shaped 
  according to the equilibrium or nonequilibrium state. A Hadamard gate is once again applied to the first qubit. The first qubit is measured. At the end 
  of the algorithm, if the magic function is in equilibrium (returns zero or one with equal probability), the result of the first qubit measurement will 
  always be zero. If the magic function is in steady state (both outcomes are returned with the same probability), the first qubit measurement result 
  will always be one.

The Deutsch Algorithm can be easily implemented with quantum computing libraries. For example, quantum computing libraries such as Qiskit provide the tools needed to implement the algorithm. For a full code example or more details about the implementation of the algorithm, you can consult the library documentation.



Grover Algorithm:

The Grover Algorithm is a quantum computing algorithm used to solve search problems of quantum computers. In particular, it is used to find a specific target input in a given function. Similar to classical algorithms, the Grover Algorithm can also be used to find the target entry in a database, but it runs faster using quantum parallelisation.

The basic working logic of the Grover Algorithm is to increase the state amplitude to find the target input within the given function, making the target state more likely. Below are the general steps of the Grover Algorithm:

In the first step, put all states into a superposition state so that the state amplitudes are equal. In the second step, invert the state of the target input to make it more probable. In the third step, make the target state more discriminable by calculating the mean value. Repeat the second step several times. With each repetition, the target state becomes more discriminable. When the algorithm is finalised, you can find the target state by measurement.
