# Hybrid Graph-Key Encryption (HGKE)
### Graph Theory meets Modular Arithmetic — a new approach to secure encryption.

---

## Overview

HGKE is a novel encryption framework that combines **Graph Theory** and **Modular Arithmetic** to build a secure, scalable, and efficient cryptographic system.

Message characters are represented as graph nodes, while modular arithmetic performs the cryptographic transformations. This hybrid design enhances security, simplifies key management, and lays a foundation for post-quantum resilient communication.

---

## The Problem

Modern encryption faces mounting pressure:

- Quantum computing threatens classical encryption methods
- Key management becomes unwieldy at scale
- Group communication systems lack efficient secure architectures
- Computational overhead grows with network size

HGKE addresses each of these by introducing graph-based key structures paired with modular arithmetic operations.

---

## How It Works

### 1. Message Representation
Each character is converted to a numerical value (A=1, B=2 ... Z=26) and becomes a **node** in a graph.

### 2. Graph Construction
Nodes are connected in message sequence, preserving character order as graph edges.
H → E → L → L → O

### 3. Key Generation
A secret key `k` is selected where:
gcd(k, 26) = 1
Valid keys: `1, 3, 5, 7, 9, 11, 15, 17, 19, 21, 23, 25`

### 4. Encryption
C = K × X (mod 26)
`X` = plaintext value · `K` = secret key · `C` = ciphertext value

### 5. Decryption
X = K⁻¹ × C (mod 26)
The modular inverse of K restores the original message, with graph connections preserving character order.

---

## System Workflow
Input → Message Conversion → Graph Construction → Key Generation

→ Encryption → Ciphertext → Secure Transmission → Decryption → Output

---

## Key Features

- Graph-based encryption with visual flow representation
- Modular arithmetic cryptographic transformations
- Dynamic key generation and management
- Scalable multi-user architecture
- Post-quantum resilience foundation

---

## Tech Stack

| Category | Tools |
|---|---|
| Language | Python |
| Graph | NetworkX, Matplotlib |
| Cryptography | math, PyCryptodome *(optional)* |
| Testing | unittest, time |

---

## Applications

- **Secure Group Communication** — corporate, academic, and team platforms
- **IoT Networks** — smart homes, healthcare devices, industrial systems
- **Data Transmission** — cloud, distributed networks, secure messaging

---

## Limitations & Future Work

**Current challenges:**
- Formal security validation pending
- Performance optimisation for real-time use
- Quantum security analysis not yet complete

**Planned enhancements:**
- Lattice-based and post-quantum cryptography integration
- Blockchain-based key distribution
- Large-scale network deployment

---

## Research References

1. *Modular Inverse Based Secured Data Transmission by the Application of Graph Theory* (2020)
2. *Graph Key-Based Encryption Technique for IoT Networks: Graph-Affine Cipher* (2023)
3. *A Graph-Based Cryptographic Framework Using Complete Graphs and Lower Triangular Identity Key Matrices* (2023)
4. *Text Encryption with Graph Theory Based Key Generation* (2024)
5. *On Graph-Based Cryptography and Symbolic Computations* (2007)

---

## Team

**Prakeya S · Harshini Sree · Thiyaanesh N R · Yuvanidhi R**

*Developed for academic and research purposes.*
