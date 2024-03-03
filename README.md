# IBM Quantum QRISE Challenge

## Title
Dynamic Circuit Challenge: Maximizing Performance and Tayloring Noise

## Background and Motivation
Dynamic circuits are an exciting feature of IBM Quantum hardware that incorporates quantum circuits with real-time classical communication. Different from the static counterpart, dynamic circuits can not only implement a set of basic quantum operations like the Hardmard gate, CNOT gate, or qubit reset but also can implement measurement in the middle of a circuit, store the measurement results to classical bits, evaluate classical expressions on the fly, and determine what quantum operation to do next. This capability has a variety of applications, for example, quantum error correction, quantum simulation, and so on. We encourage you to explore what you can do with dynamic circuits in this challenge! Bonus point if you show improvement of your dynamic circuit implementation over its static counterpart - for example, use dynamic circuit feature to shorten the circuit depth, suppress error rate, and so on! After you create a dynamic circuit of your interest and are ready to run it on the hardware, bear in mind that the current quantum computers are noisy! In practical implementation, the operations in a dynamic circuit can be faulty, so it is important to quantify their fidelities and model the noise mechanism on their own or in the context of a circuit. In the case of dynamic circuits, the types of error and how error propagates will be more complicated due to the hybrid quantum and classical nature of noise! We challenge you to characterize the noise in dynamic circuits. Fortunately, there is a suite of noise characterization and verification tools like tomography and randomized benchmarking, which are fairly well understood on static circuits, and extending them to dynamic circuits is an interesting research question to take on.

## Challenge Prompts
1. Find an application using dynamic circuits
*For example:prepare a large GHZ state, generate long-range entanglement, prepare a repetition code, doing quantum phase estimation.*
2. Demonstrate the improvement of implantation using the dynamic circuit feature
*For example: use dynamic circuit feature to shorten circuit depth or suppress error rate in a real circuit execution*
3. Characterize noise and errors in dynamic circuits
*For example, study how error propagates in dynamic circuits: use a benchmark method to study
the fidelities of individual operations and composite operations in dynamic circuits*
4. With deeper understanding of how noise affects dynamic circuits, could you think of ways to suppress noise?

## Getting Started Resources
1. What are dynamic circuits? Find out from the IBM’s blog post [here](https://www.ibm.com/quantum/blog/quantum-dynamic-circuits).
2. Documentation on dynamic circuits [here](https://docs.quantum.ibm.com/build/classical-feedforward-and-control-flow)
3. For testing and debugging the quantum circuits locally, the [qiskit_aer](https://github.com/Qiskit/qiskit-aer) simulators can be useful
4. Further reading about dynamic circuits
    1. [Exploiting Dynamic Quantum Circuits in a Quantum Algorithm with Superconducting Qubits](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.127.100501)
    2. [Efficient Long-Range Entanglement using Dynamics Circuits](https://arxiv.org/pdf/2308.13065.pdf)
    3. [A randomized benchmarking suite for mid-circuit measurements](https://iopscience.iop.org/article/10.1088/1367-2630/ad0e19)

## Submission criteria
The submission could be software, a presentation, a video, a written document, a wiki page, a blog post, or any combination. Your work should ideally use or discuss dynamic circuits. We encourage you to run it on the IBM hardware! If you do, a circuit for an interesting application with a larger number of qubits and better overall fidelity is always more desirable.


