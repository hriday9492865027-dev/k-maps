# 🗺️ K-Map Solver & Logic Lab

An interactive **Karnaugh Map (K-Map) Solver & Minimizer** and **Matrix Multiplication Trace Visualizer** with modern dark aesthetics.

---

## ✨ Features

### 1. 🗺️ Karnaugh Map (K-Map) Solver
- **2, 3, and 4 Variables:**
  - 2-Var ($A, B$): 4 cells
  - 3-Var ($A, B, C$): 8 cells with Gray-coded columns ($00, 01, 11, 10$)
  - 4-Var ($A, B, C, D$): 16 cells with Gray-coded rows & columns
- **Optimization Modes:** SOP (Sum of Products) & POS (Product of Sums).
- **Don't-Care ($X$) Handling:** Optional inclusion in prime implicant groups.
- **Multiple Input Methods:**
  - **Boolean Expression Parser:** Enter expressions like `A'B + B'CD + A*B*C'`, `A ^ B ^ C`, etc.
  - **Interactive Cell Toggling:** Click any cell to cycle `0 → 1 → X → 0`.
  - **Quick Presets:** Full Adder Sum/Carry, Majority Gate, 2:1 MUX, 4-Bit XOR Parity, BCD Segment A.
  - **Toolbar:** Random Fill, Clear (0), Fill (1), and Invert.
- **Visual Grouping Rectangles:** Overlaid grouping blocks with support for edge-wrapping and 4 corners.
- **Interactive Spotlight:** Hovering over a term in the simplified equation spotlights the group on the map.
- **Detailed Step-by-Step Explanation:**
  - Truth table & minterm mapping ($m_0, m_1, \dots$).
  - Power-of-2 Gray code grouping.
  - Variable-by-variable elimination trace ($0 \to 1 \implies$ eliminated).
  - Essential Prime Implicant (EPI) verification.
  - Hardware RTL Verilog and C bitwise logic exports.
  - Logic gate savings percentage.

### 2. 🔢 Matrix Multiplication Trace Visualizer
- Visualizes step-by-step dot product calculation: $C[i][j] = \sum A[i][k] \times B[k][j]$.
- Step controls: Play, Pause, Step Forward/Backward, and Speed adjustment.
- Dynamic matrix dimensions and value editing.

---

## 🚀 Getting Started

Simply open `index.html` (or `k map.html`) in your browser or with **Live Server** in VS Code.
