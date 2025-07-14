

\# Quantum Climate Risk Insurance – Phase 3 Submission



\*\*Team Name\*\*: Feeltech  

\*\*Project Title\*\*: Quantum Climate Risk Insurance  

\*\*Challenge Track\*\*: Quantum-Enhanced Risk Assessment \& Prediction (World Bank)



---



\## 🚀 Launch on qBraid



[<img src="https://qbraid-static.s3.amazonaws.com/logos/Launch\_on\_qBraid\_black.png" width="150">](https://account.qbraid.com?gitHubUrl=https://github.com/kkoci/WorldBank\_QuantumRiskAssessment)



---



\## 🛠 Setup Instructions



This project runs entirely on Python using Qiskit and standard data science packages. All code is organized in Jupyter Notebooks.



\### Environment Dependencies



You can run this project on \[qBraid](https://account.qbraid.com) without needing local installation. If running locally, ensure the following packages are installed:



&nbsp;   pip install qiskit numpy pandas matplotlib seaborn scikit-learn



---



\## 📂 Repository Structure



\- `WorldBank\_simulation.ipynb`: Main notebook used for Phase 3 results. Executes simulation of the quantum circuit using Qiskit Aer with realistic noise modeling. This is the core submission notebook.

\- `WorldBank\_realHw.ipynb`: Identical logic, adapted to run on IBM's real hardware backend (`ibm\_brisbane`). Included for reference and future validation.

\- `screenshots/`: Folder containing evidence of long wait queues and hardware job submission status for `ibm\_brisbane`.

\- `README.md`: This file.

\- `writeup.pdf`: 4-page technical report (in separate file).



---



\## ▶️ How to Run on qBraid



1\. Click the \*\*Launch on qBraid\*\* button above.  

2\. Open and run the notebook `WorldBank\_simulation.ipynb`.  

3\. All climate data is generated and processed in-notebook (no `.xlsx` file required).  

4\. Run cells in sequence to complete the workflow: feature processing → quantum circuit → output metrics.



---



\## 📥 Expected Inputs \& Outputs



\- \*\*Inputs\*\*: Synthetic climate features (temperature, precipitation, cyclone intensity) scaled from real-world data ranges.  

\- \*\*Outputs\*\*:  

&nbsp; - Calibrated flood risk classification  

&nbsp; - Quantum-informed premium pricing  

&nbsp; - Accuracy and performance evaluation vs. classical baseline



---



\## ⚖️ Hardware Constraints and Simulation Note



Due to persistent queue saturation and long delays on IBM’s `ibm\_brisbane` quantum backend, we executed the final evaluation using \*\*Qiskit Aer simulators\*\* with realistic noise modeling to approximate hardware behavior.



The companion file `WorldBank\_realHw.ipynb` includes all code necessary to run the same model on actual IBM Q hardware and is validated for execution compatibility.



To document these hardware access limitations, we have included a `screenshots/` folder showing wait times and backend status at the time of submission.



---



\## 🚧 Known Limitations



\- Real-time dataset (`Bangladesh\_FloodRisk\_Features\_2024.xlsx`) is embedded in-code; no separate file required.  

\- Execution on real quantum hardware is delayed due to high queue times, but notebook is validated and compatible.  

\- Simulator results approximate near-term NISQ behavior but may differ slightly from real QPU output under decoherence.



---



\## ✅ Summary



This project delivers a working hybrid quantum-classical model for flood risk prediction and insurance premium pricing, aligned with real-world actuarial needs. While final simulations were run on noise-modeled Qiskit Aer, the design is hardware-ready and reproducible on qBraid or IBM Q.



