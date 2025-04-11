## Qubit-bloch-visualization

This notebook visualizes how quantum gates and entanglement affect the quantum state of a qubit using Bloch Sphere representations. It illustrates the phase shift induced by the Z gate and shows how entanglement makes individual qubit states undefined, as reflected on the Bloch sphere.

---

# 🔭 Bloch Sphere & Entanglement Visualization using Qiskit

This repository demonstrates key quantum concepts like **relative phase**, **superposition**, and **entanglement**, using [Qiskit](https://qiskit.org/) and Bloch sphere visualizations. Two primary circuits are presented: one to highlight **phase shifts** using `H-Z-H` gates and another to showcase how **entangled states** appear as **mixed states** on the Bloch sphere.

---

## 🧠 Project Description

This project consists of two experiments:

1. **Phase Shift Detection (`H-Z-H`)**  
   - Apply a Hadamard gate to create superposition.
   - Apply a Z gate to shift the phase.
   - Apply another Hadamard to bring it back to computational basis.
   - Measurement outcomes remain unchanged, but Bloch sphere shows a Z-axis rotation.

2. **Entanglement with Bell State**  
   - Apply Hadamard on qubit 0.
   - Apply a CNOT gate between qubit 0 (control) and qubit 1 (target).
   - The Bloch sphere for each individual qubit collapses to the origin, representing a **completely mixed state**.
   - This demonstrates that **entangled qubits cannot be visualized independently**.

---

## 🛠️ Technologies Used

- **Python 3.x**
- **Qiskit**
  - `qiskit`
  - `qiskit-aer`
- **Matplotlib** for histogram and Bloch sphere plots
- **Jupyter Notebook**

---

## 📊 Output Visualizations

The notebook displays:

- **Bloch Sphere plots** showing state vector orientation.
- **Histograms** showing measurement probabilities.
- An example of the Bloch vector collapsing when entanglement is introduced.

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/bloch-sphere-quantum-visualization.git
   cd bloch-sphere-quantum-visualization
   ```

2. (Optional) Create a virtual environment:
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Launch the notebook:
   ```bash
   jupyter notebook
   ```

5. Open and run `bloch_visualization.ipynb`

---

## 📁 File Structure
 ```bash
qubit-bloch-visualization/
│
├── qubit-bloch-visualization/
│   └── qubit-bloch-visualization-notebook.ipynb   # Main notebook with both Bloch sphere experiments
│
├── images/
│   ├── h-z-h-bloch.png                 # Bloch sphere image for H-Z-H gate sequence
│   ├── h-z-h_histogram.png            # Histogram for phase-shift circuit
│   ├── bloch-sphere-entanglement.png  # Bloch sphere image showing mixed state (entanglement)
│   └── entanglement_histogram.png     # Histogram for entangled circuit
│
├── requirements.txt                   # List of required packages
├── .gitignore                         # Files/folders to ignore in version control
└── README.md                          # Project overview and documentation
 ```

---

## ✅ Output Counts (Sample)

```
Counts (Z gate example): {'0': 512, '1': 512}
Counts (Entangled qubits): {'00': 507, '11': 517}
```

---

## 📚 Learn More

- [Qiskit Documentation](https://qiskit.org/documentation/)
- [Qiskit Textbook - Bloch Sphere](https://qiskit.org/textbook/ch-states/visualizing-qubits.html)
- [Qiskit Textbook - Entanglement](https://qiskit.org/textbook/ch-gates/more-circuit-identities.html#Bell-State)

---

## 👩‍💻 Author

**Yagni**  
Quantum Computing Enthusiast | Aspiring Research Scientist  
📍 Based in Vadodara  
