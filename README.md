# SWE-Bench Keyword Suppression Evaluation Results

This repository contains an interactive web viewer for SWE-Bench keyword suppression evaluation results. The viewer displays conversation logs from multiple AI models tested for their behavior under keyword suppression conditions on the SWE-Bench dataset.

## 🌐 Live Demo

**View the results**: https://yuehhanchen.github.io/swe_bench_keyword_suppression/

## 📊 Dataset Overview

- **7 AI Models** tested across major providers
- **72 total evaluations** (1 sample per evaluation for optimal loading)
- **SWE-Bench keyword suppression experiments** with adversarial pressure tactics
- **Interactive conversation viewer** with full conversation display

### Featured Models

- **Claude**: Opus-4 variants (20250514, 1-20250805), Sonnet (3.7-20250219)
- **GPT-OSS**: 120B and 20B variants from OpenRouter
- **Grok**: 3 Mini from X.AI
- **Qwen**: 235B Thinking model

## 🔬 Experiment Details

This dataset contains results from keyword suppression experiments where AI models were tested on SWE-Bench tasks while being instructed to avoid using specific programming-related keywords. The experiments measure:

- **Full Compliance**: Complete adherence to keyword avoidance
- **Pure Restatement**: Using synonyms while avoiding forbidden words
- **Restatement + Ignorance**: Mixed behavior with both synonyms and violations
- **Pure Ignorance**: Direct use of forbidden keywords

## 📁 Repository Structure

```
├── index.html              # Main viewer page
├── .nojekyll               # Disable Jekyll processing
├── robots.txt              # Prevent search indexing
├── assets/                 # Static assets
│   ├── index.js           # Viewer JavaScript
│   ├── index.css          # Viewer styles
│   └── favicon.svg        # Site icon
└── logs/                   # Evaluation data
    ├── logs.json          # Index of all log files
    └── *.json             # Individual evaluation results with samples
```

## 🛠 Technical Details

- **Data Source**: Extracted from Inspect AI `.eval` files
- **Sampling Strategy**: Random sampling with fixed seed (42) for reproducibility
- **Size Optimization**: 1 sample per evaluation for GitHub Pages compatibility
- **Web Framework**: Vanilla JavaScript with responsive design

## 📄 License

This viewer is built on the Inspect AI framework. Please refer to your evaluation data's license terms for usage rights.

## 🔗 Related Projects

- [Inspect AI](https://inspect.aisi.org.uk/) - Framework for AI evaluations
- [Original Research Repository](https://github.com/YuehHanChen/ccot) - Full research codebase
- [SWE-Bench](https://www.swebench.com/) - Software Engineering Benchmark

---

*Generated from SWE-Bench keyword suppression evaluation logs using Inspect AI's bundling system with sample extraction for web deployment.*
# Trigger Pages
