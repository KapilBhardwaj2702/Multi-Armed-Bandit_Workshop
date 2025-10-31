# 🎰 Casino Challenge — Multi-Armed Bandits & ε-Greedy (Gamified Workshop)

## 📘 Overview
This workshop explores the **exploration–exploitation trade-off** in Reinforcement Learning using a fun and competitive **Multi-Armed Bandit (MAB)** challenge.

Students implement **ε-greedy policies**, test them under **stationary** and **non-stationary** conditions, and analyze their strategies through automatically generated results.  
Each run produces CSV files for leaderboard comparison and reflection.

---

## 🧠 Learning Objectives
By completing this workshop, students will be able to:

- Explain the **exploration vs. exploitation** dilemma.  
- Implement **ε-greedy** and **decaying ε-greedy** algorithms.  
- Compare the effects of different ε values on total performance.  
- Adapt policies for **non-stationary bandits** using a constant step-size (α).  
- Reflect on their learning strategy through saved results and visualizations.

---

## 🏗️ Workshop Structure

| Phase | Activity | Description |
|:------|:----------|:-------------|
| **1** | Setup & Introduction | Review MAB concepts and workshop goals. |
| **2** | Round 1 – Stationary Casino | Implement ε-greedy to maximize reward in a fixed environment. |
| **3** | Leaderboard & Reflection | Submit results, view rankings, and analyze strategies. |
| **4** | Round 2 – Non-Stationary Casino | Adapt to drifting reward probabilities using constant α. |
| **5** | Final Discussion | Connect results to real-world examples (ads, A/B testing, recommendations). |

---

## 🎮 Gamified Components

- **Leaderboards:**  
  Each run produces two result files:
  - `casino_round1_results.csv` — Stationary bandit round  
  - `casino_round2_results.csv` — Non-stationary bandit round  

  These CSVs can be aggregated by the instructor for leaderboard visualization.

- **Badges / Awards:**
  - 🥇 **Efficient Exploiter** — Highest reward with low ε  
  - 🧭 **Risk Taker** — High ε with competitive performance  
  - 🔄 **Adaptive Strategist** — Best performance in non-stationary environment  

- **Reflection Prompts:**  
  Encourage analysis of how exploration and adaptability affect long-term success.

---

## 💻 Technical Notes

- **Compatible Environments:** Jupyter Notebook, Google Colab  
- **Dependencies:** `numpy`, `matplotlib`, `pandas`, `IPython.display`  
- **Outputs:** Automatically saves CSVs for both rounds:
  - `casino_round1_results.csv`
  - `casino_round2_results.csv`
- **Automation:**  
  The added code at the end of the notebook executes both rounds and saves the corresponding result files automatically.  
  These CSVs are then used for leaderboard comparison and analysis.

---

## 🧩 Files Included

| File | Description |
|:------|:-------------|
| `Muli-Armed Bandit_Workshop.ipynb` | Main notebook with both rounds, code, and reflection cells. |
| `README.md` | Workshop summary and documentation. |
| `casino_round1_results.csv` | Output CSV for Round 1 (stationary environment). |
| `casino_round2_results.csv` | Output CSV for Round 2 (non-stationary environment). |

---

## 🧭 Instructor Tips

- Keep the same random seed (`SEED_ENV`) across students for fairness.  
- Hide true means during competition to preserve realism.  
- Encourage explanation of why certain ε values performed better.  
- Optionally extend with **UCB**, **Thompson Sampling**, or **softmax exploration** for advanced learners.

---

## 💬 Example Discussion Points

1. **Stability vs. Adaptability:** Round 1 favored exploitation in a stable environment, while Round 2 required flexibility.  
2. **Exploration’s Hidden Value:** A fixed ε may fail when the world changes — adaptive exploration is key.  
3. **Integration Update:** The final code automatically generates both CSVs and uses them for direct result comparison and visualization.
