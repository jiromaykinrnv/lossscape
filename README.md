# lossscape

Minimal training loop I use to test ideas fast

## Highlights

- Metrics logged to CSV for plotting
- Synthetic dataset mode: no download needed to smoke-test
- Single file model definition, easy to hack
- Cosine LR schedule with warmup
- Gradient clipping and clean metrics logging

## Installation

```bash
pip install -r requirements.txt
```

## Usage

```bash
python train.py --epochs 5 --synthetic
# metrics land in runs/metrics.csv
```

## Project structure

```text
├── docs/
│   ├── development.md
│   ├── roadmap.md
│   └── usage.md
├── .editorconfig
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── SECURITY.md
├── model.py
├── requirements.txt
└── train.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
```

## FAQ

**Is this production ready?**  
It works for my use case; review the code before relying on it.

**Why no framework?**  
The stdlib covers what this project needs.
