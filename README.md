# QR-Playbook

> Quantitative Research Playbook – a structured portfolio of models and tools for quantitative finance.
> Includes option pricing, stochastic simulations, calibration routines, Monte Carlo methods, and PDE solvers, implemented in Python (and C++ extensions).

---

## 📌 Overview

This repository is a hands-on collection of core quantitative finance models and numerical methods.
It is designed as both a **learning project** and a **demonstration portfolio** for quantitative research and development roles.

Key domains covered:

* **Option Pricing** (Black–Scholes, Greeks, Binomial/Trinomial Trees, IR Curve Bootstrap)
* **Stochastic Simulation** (Euler–Maruyama, Milstein, GBM, OU, CIR processes)
* **Model Calibration** (Least-Squares, Heston, SABR with constraints)
* **Monte Carlo Methods** (Antithetic, Stratified, Sobol quasi-MC; Greeks via Pathwise & Likelihood Ratio)
* **PDE Solvers** (Crank–Nicolson for BS PDE, Barrier Options)
* **Testing & CI** (pytest, reproducible results, CI-ready)

---

## 📂 Repository Structure

```
QR-Playbook/
│
├── pricing/         # Black–Scholes, Greeks, trees, yield curve bootstrap
├── stoch_sim/       # SDE simulation library (Euler, Milstein, GBM, OU, CIR)
├── calibration/     # Model calibration (Heston, SABR, constraints)
├── mc/              # Monte Carlo methods + variance reduction
├── pde/             # PDE solvers (Crank–Nicolson, barriers)
├── tests/           # pytest unit tests + CI setup
└── README.md        # Project documentation
```

---

## 🚀 Getting Started

### Requirements

* Python 3.10+
* NumPy, SciPy, Matplotlib, Pandas
* [pytest](https://docs.pytest.org/) for testing
* (Optional) C++17 + Eigen for performance-critical modules

### Installation

Clone the repo:

```bash
git clone https://github.com/<your-username>/QR-Playbook.git
cd QR-Playbook
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run tests:

```bash
pytest
```

---

## 📘 Usage Examples

```python
from pricing.black_scholes import black_scholes_price

price = black_scholes_price(S0=100, K=100, T=1, r=0.05, sigma=0.2, option_type="call")
print(f"European Call Price: {price:.4f}")
```

More usage demos can be found in the [`examples/`](examples/) folder (planned).

---

## 🛠 Roadmap

* [ ] Add American option pricing via finite differences
* [ ] Extend SDE library with jump-diffusion models (Merton, Kou)
* [ ] Implement XVA-light module (CVA/DVA approximations)
* [ ] Build Jupyter notebooks with visualizations
* [ ] Add performance benchmarking (Python vs C++)

---

## 🧪 Testing & CI

* Each module includes **unit tests** under `tests/`
* CI setup with GitHub Actions (planned)
* Code coverage reports (planned)

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome!
Fork the repo, create a feature branch, and submit a PR.

---

## 👤 Author

**Maria Sole Olivieri**
MSc in Statistical Methods & Applications (Quantitative Economics)
📍 Europe | Aspiring Quant Researcher
