# Hybrid Graph-Key Encryption (HGKE)

## Overview

Hybrid Graph-Key Encryption (HGKE) is a novel encryption framework that combines Graph Theory and Modular Arithmetic to create a secure, scalable, and efficient encryption system.

The project introduces a graph-based key management approach where message characters are represented as graph nodes, while modular arithmetic is used to perform cryptographic transformations. This hybrid design enhances security, simplifies key management, and provides a foundation for future post-quantum secure communication systems.

---

## Abstract

In modern communication systems, secure data transmission and efficient key management remain critical challenges. Traditional encryption methods often struggle with scalability and may become vulnerable to future quantum computing attacks.

Hybrid Graph-Key Encryption (HGKE) addresses these challenges by integrating graph structures with modular arithmetic-based encryption techniques. The system provides:

- Enhanced confidentiality
- Secure key management
- Efficient encryption and decryption
- Scalability for multi-user environments
- Potential resistance against future quantum attacks

---

## Problem Statement

Current encryption systems face several challenges:

- Vulnerability to emerging quantum attacks
- Complex key management for large networks
- Limited scalability in group communication systems
- Increased computational overhead in secure communication

HGKE aims to solve these problems by introducing graph-based key structures combined with modular arithmetic operations.

---

## Objectives

### Enhanced Security

Develop a secure encryption framework using graph theory and modular arithmetic.

### Novel Key Management

Introduce graph-based cryptographic key generation and distribution.

### Operational Efficiency

Achieve secure encryption while maintaining practical computational performance.

### Post-Quantum Resilience

Provide a foundation for future encryption systems capable of resisting quantum computing threats.

---

## Key Features

- Hybrid Graph-Based Encryption
- Modular Arithmetic Cryptography
- Dynamic Key Management
- Secure Group Communication
- Scalable Architecture
- Graph Visualization of Encryption Flow
- Efficient Encryption and Decryption
- Future-Ready Security Design

---

## Methodology

### Step 1: Message Representation

Each character of the message is converted into a numerical value:

```text
A = 1
B = 2
...
Z = 26
```

Each character becomes a node in a graph.

### Step 2: Graph Construction

Nodes are connected according to message sequence and relationships.

Example:

```text
H → E → L → L → O
```

Graph edges preserve character order and structure.

### Step 3: Key Generation

A valid secret key `k` is selected such that:

```text
gcd(k, 26) = 1
```

Example valid keys:

```text
1, 3, 5, 7, 9, 11, 15, 17, 19, 21, 23, 25
```

### Step 4: Encryption

Encryption Formula:

```text
C = K × X (mod 26)
```

Where:

- X = Plaintext value
- K = Secret key
- C = Ciphertext value

### Step 5: Graph Mapping

The encrypted values remain associated with graph nodes.

Graph topology adds an additional security layer.

### Step 6: Decryption

Decryption Formula:

```text
X = K⁻¹ × C (mod 26)
```

Where:

- K⁻¹ = Modular inverse of K

The original message order is restored using graph connections.

---

## System Workflow

```text
User Input
     │
     ▼
Message Conversion
     │
     ▼
Graph Construction
     │
     ▼
Key Generation
     │
     ▼
Encryption
     │
     ▼
Ciphertext Output
     │
     ▼
Secure Transmission
     │
     ▼
Decryption
     │
     ▼
Original Message
```

---

## Technologies Used

### Programming Language

- Python

### Cryptography Libraries

- math
- cryptography (optional)
- PyCryptodome (optional)

### Graph Libraries

- NetworkX
- Matplotlib

### Testing Tools

- unittest
- time

---

## Applications

### Secure Group Communication

- Corporate Communication
- Team Collaboration Systems
- Educational Platforms

### Internet of Things (IoT)

- Smart Homes
- Healthcare Devices
- Industrial IoT Networks

### Secure Data Transmission

- Cloud Systems
- Distributed Networks
- Secure Messaging Applications

---

## Advantages

- Strong Security
- Scalable Key Management
- Efficient Encryption
- Graph-Based Complexity
- Easy Key Distribution
- Future Quantum-Resistant Potential
- Suitable for Multi-User Systems

---

## Challenges

- Formal Security Validation
- Performance Optimization
- Real-Time Implementation
- Quantum Security Analysis

---

## Future Enhancements

- Integration with Post-Quantum Cryptography
- Lattice-Based Encryption Support
- Blockchain-Based Key Distribution
- Real-Time Secure Communication Systems
- Large-Scale Network Deployment

---

## Research References

1. Modular Inverse Based Secured Data Transmission by the Application of Graph Theory (2020)
2. Graph Key-Based Encryption Technique for IoT Networks: Graph-Affine Cipher (2023)
3. Some Graph-Based Encryption Techniques
4. A Graph-Based Cryptographic Framework Using Complete Graphs and Lower Triangular Identity Key Matrices (2023)
5. Text Encryption with Graph Theory Based Key Generation (2024)
6. On Graph-Based Cryptography and Symbolic Computations (2007)

---

## Team Members

- Prakeya S
- Harshini Sree
- Thiyaanesh N R
- Yuvanidhi R

---

## License

This project is developed for academic and research purposes.
