# From Neural Tokens to Language

Code and experiments for the paper **From Neural Tokens to Language**.
Official implementation of the paper **"From Neural Tokens to Language: Dual-View EEG Semantic Bridging for Brain-to-Text Generation"**.

This repository contains the code and resources for EEG-based semantic representation learning and brain-to-text generation. The project is organized around an EEG encoder, multimodal semantic bridging modules, and large language / CLIP model components.

## Repository Structure

```text
From-Neural-Tokens-to-Language/
|-- README.md
|-- dataset/
|   |-- raw/
|   |-- processed/
|   `-- README.md
|-- channelnet/
|   |-- __init__.py
|   |-- model.py
|   |-- layers.py
|   `-- utils.py
|-- models/
|   |-- clip/
|   |-- llm/
|   `-- README.md
|-- scripts/
|   |-- preprocess.py
|   |-- train.py
|   `-- evaluate.py
|-- configs/
|   `-- default.yaml
`-- requirements.txt
```

## Directory Description

- `dataset/`: Stores the EEG-text dataset used by the project.
  - `dataset/raw/`: Original downloaded or collected data.
  - `dataset/processed/`: Preprocessed EEG signals, aligned text, and training-ready files.

- `channelnet/`: Contains the EEG encoder model code.
  - This directory is intended for ChannelNet-style EEG feature extraction modules, encoder layers, and related utilities.

- `models/`: Stores large language model and CLIP-related model components.
  - `models/clip/`: CLIP model wrappers, visual/text semantic embedding utilities, or downloaded CLIP checkpoints.
  - `models/llm/`: Large language model wrappers, tokenizer utilities, generation modules, or downloaded LLM checkpoints.

- `scripts/`: Training, preprocessing, and evaluation entry points.

- `configs/`: Experiment configuration files.

## Data

Place all datasets under the `dataset/` directory. Large raw data files and generated processed files should not be committed directly to GitHub unless they are small metadata files or sample files required to run a minimal example.

Recommended layout:

```text
dataset/
|-- raw/
|-- processed/
`-- README.md
```

## Overview
## Models

This repository will contain the implementation, experiment scripts, and supporting materials for the paper.
Place CLIP and large language model files under the `models/` directory. If model checkpoints are too large for GitHub, please provide download instructions in `models/README.md` instead of committing the checkpoint files directly.

## Repository Structure
Recommended layout:

```text
.
├── README.md
└── .gitignore
models/
|-- clip/
`-- llm/
```

## Installation

```bash
git clone https://github.com/wanfkuabc/From-Neural-Tokens-to-Language.git
cd From-Neural-Tokens-to-Language
pip install -r requirements.txt
```

## Usage

The full training and evaluation pipeline will be released with the paper code.

Example workflow:

```bash
python scripts/preprocess.py --config configs/default.yaml
python scripts/train.py --config configs/default.yaml
python scripts/evaluate.py --config configs/default.yaml
```

## Citation

Citation information will be added when available.
If you find this repository useful, please cite our paper:

```bibtex
@article{from_neural_tokens_to_language,
  title={From Neural Tokens to Language: Dual-View EEG Semantic Bridging for Brain-to-Text Generation},
  author={},
  journal={},
  year={2026}
}
```

## License

The license will be added later.
