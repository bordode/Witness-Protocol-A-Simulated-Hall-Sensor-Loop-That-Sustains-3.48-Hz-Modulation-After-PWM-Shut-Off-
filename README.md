# Witness-Protocol-A-Simulated-Hall-Sensor-Loop-That-Sustains-3.48-Hz-Modulation-After-PWM-Shut-Off-
Simulation-only code that demonstrates a solver-induced ‘ghost’ frequency; use it to test feedback-loop stability, not to claim new physics
Witness Protocol: A Simulated Hall-Sensor Loop That Sustains 3.48 Hz Modulation After PWM Shut-Off — A Numerical Artefact Study”Simulation-only code that demonstrates a solver-induced ‘ghost’ frequency; use it to test feedback-loop stability, not to claim new physics

“algorithmic artefact + cautionary tale”
repo:  witness-protocol-simulation
├── README.md               # lead with “SIMULATION ONLY – no physical coils were built”  
├── src/
│   ├── hall_feedback.cpp   # the KiSS-SIDM + Hall lookup loop  
│   └── analysis.ipynb      # FFT that shows 3.48 Hz persistence  
├── data/
│   ├── isolation_run.csv   # the synthetic Hall trace  
│   └── MANIFEST.sha256     # hash of raw numbers  
├── docs/
│   ├── witness_report.pdf  # short methods paper (2 pages)  
│   └── replication.md      # step-by-step for anyone to re-run  
└── LICENSE                 # MIT – invite forks, require citation

“Witness Protocol – Simulation of a Hall-sensor feedback loop that spontaneously produces a 3.48 Hz beat after artificial PWM shut-off. This is a numerical artefact, not a physical measurement. Use it to test solver stability, not to claim new physics.”# Witness Protocol  
> Simulation of a Hall-sensor feedback loop that sustains 3.48 Hz modulation after PWM shut-off — a numerical artefact study  

![GitHub release](https://img.shields.io/github/v/release/yourname/witness-protocol-simulation)  
![License](https://img.shields.io/badge/license-MIT-blue.svg)  
![Python](https://img.shields.io/badge/python-3.9+-blue.svg)  

## ⚠️  In a nutshell  
- **No physical hardware was built** — everything is synthetic.  
- The “ghost” frequency is an emergent beat in the KiSS-SIDM solver + Hall lookup table.  
- Use this repo to **test non-linear solver stability** or **reproduce the artefact**.  

## 🚀  Quick start (30 s)
```bash
git clone https://github.com/yourname/witness-protocol-simulation.git
cd witness-protocol-simulation
pip install -r requirements.txt
python -m src.run_protocol

Keep the README one-screen, crystal-clear; add three small badges and a 30-second “how to run” — that’s all GitHub surfers need.

```markdown
# Witness Protocol  
> Simulation of a Hall-sensor feedback loop that sustains 3.48 Hz modulation after PWM shut-off — a numerical artefact study  

![GitHub release](https://img.shields.io/github/v/release/yourname/witness-protocol-simulation)  
![License](https://img.shields.io/badge/license-MIT-blue.svg)  
![Python](https://img.shields.io/badge/python-3.9+-blue.svg)  

## ⚠️  In a nutshell  
- **No physical hardware was built** — everything is synthetic.  
- The “ghost” frequency is an emergent beat in the KiSS-SIDM solver + Hall lookup table.  
- Use this repo to **test non-linear solver stability** or **reproduce the artefact**.  

## 🚀  Quick start (30 s)
```bash
git clone https://github.com/yourname/witness-protocol-simulation.git
cd witness-protocol-simulation
pip install -r requirements.txt
python -m src.run_protocol
```

Output: `isolation_trace.csv` + FFT plot showing 3.48 Hz peak.

📊  What you get
- Raw synthetic Hall-sensor trace (1 kHz)  
- Jupyter notebook that reproduces the FFT figure  
- MIT licence — fork and modify freely  

📜  Cite
If you use this code, please cite:

“Witness Protocol: A Numerical Artefact Study”, GitHub DOI: 

🤝  Contributing
Issues and pull requests welcome — especially hardware-in-the-loop replications that confirm or refute the beat frequency.  

📧  Contact
bordode@gmail.com
