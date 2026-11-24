# CMPE 260 — Project 2: Policy Gradient on Atari Pong

A three-way comparison of DQN, REINFORCE, and A2C on the ALE/Pong-v5 environment.

## Team
| Member | Responsibility |
|--------|---------------|
| Dev Mulchandani | Environment setup, REINFORCE implementation |
| Kalhar Patel | REINFORCE hyperparameter tuning |
| Deep Dhaduk | A2C architecture and tuning |
| Nikita Memane | DQN bridge, three-way comparison, evaluation |

## Repository Structure
```
Project 2/
├── code/              # Jupyter notebook with full pipeline
├── figures/           # Training curves, evaluation plots, bias diagnostics
├── presentation/      # 17-slide presentation (matched to Project 1 template)
├── report/            # IEEE-format project report (PDF)
└── results/           # Training summaries and CSVs
```

## Key Results
| Algorithm | Final Mean-100 | Eval (30 ep) | Convergence |
|-----------|---------------|-------------|-------------|
| DQN (Project 1) | 19.55 | 21.00 | ~1.25M steps |
| REINFORCE | -20.07 | -21.00 | Not reached |
| A2C | -20.68 | -21.00 | Not reached |

## How to Run
1. Open `code/CMPE260_Project2_PolicyGradient_Pong-2.ipynb` in Google Colab
2. Select a T4 GPU runtime
3. Run all cells (cached results load from Google Drive; full retraining takes ~2 hours)

## Hardware
- DQN (Project 1): NVIDIA L4 GPU
- REINFORCE and A2C (Project 2): Tesla T4 GPU (Google Colab)
