# Pharmacometrics Benchmarks

A curated collection of benchmark datasets for evaluating pharmacometric modeling methodologies.

## 🎯 Purpose

This repository is being developed as a collection of documented pharmacometric benchmark datasets that will enable:

- Reproducible comparison of different modeling approaches
- Transparent evaluation of new methods
- Community-driven standards for pharmacometrics
- Competitive innovation through organized challenges

## 🌐 Website

Visit our [GitHub Pages site](https://aiml-sig.github.io/pmx_benchmarks/) for:

- Complete documentation
- Browse the reference example and future community benchmarks
- Submission guidelines
- Contact information

## 📊 Benchmark Example

The [benchmark page](https://aiml-sig.github.io/pmx_benchmarks/benchmarks.html) currently contains a reference example. Community submissions are welcome.

## 🚀 Quick Start

### Using Benchmarks

Data files can be accessed directly from this repository. Install Git LFS and run `git lfs pull` after cloning to retrieve CSV data rather than pointer files. The current files illustrate the format; they are not a complete scientific benchmark.

```python
# Python example - direct access
import pandas as pd

# Load a benchmark dataset
train = pd.read_csv('benchmarks/example-pk-model-selection/data/train.csv', na = c('', 'NA', '.'))
test = pd.read_csv('benchmarks/example-pk-model-selection/data/test.csv', na = c('', 'NA', '.'))
```

```r
# R example - direct access
library(readr)

# Load a benchmark dataset
train <- read_csv('benchmarks/example-pk-model-selection/data/train.csv', na = c('', 'NA', '.'))
test <- read_csv('benchmarks/example-pk-model-selection/data/test.csv', na = c('', 'NA', '.'))
```

### Helper Packages

Helper packages for Python, R, and Julia are proposals, not available releases. See [COMPANION_REPOS.md](COMPANION_REPOS.md) to help develop them.

### Submitting a Benchmark

1. Fork this repository
2. Create your benchmark in `benchmarks/<your-dataset-name>/`
3. Follow the structure in `benchmarks/example-pk-model-selection/`
4. Submit a Pull Request

See our [submission guide](https://aiml-sig.github.io/pmx_benchmarks/submission-guide.html) for detailed instructions.

## 📁 Repository Structure

```
pmx_benchmarks/
├── benchmarks/              # Benchmark datasets
│   └── <dataset-name>/
│       ├── index.qmd        # Documentation
│       ├── metadata.yml     # Machine-readable metadata
│       ├── data/
│       │   ├── train.csv
│       │   ├── test.csv
│       │   └── data-dictionary.yml
│       └── README.md
├── .github/
│   ├── workflows/          # CI/CD workflows
│   ├── scripts/            # Validation scripts
│   └── PULL_REQUEST_TEMPLATE.md
├── _quarto.yml             # Quarto configuration
├── index.qmd               # Website homepage
├── about.qmd               # About the initiative
├── submission-guide.qmd    # Submission guidelines
├── benchmarks.qmd          # Benchmark listings
├── contact.qmd             # Contact information
└── README.md               # This file
```

## 🔍 Benchmark Goals

There are two submission tracks — see the [Scope & Eligibility](https://aiml-sig.github.io/pmx_benchmarks/scope.html) page for details.

**Goal 1 — Generic Benchmarks:** Teaching cases, agentic datasets, unit-test style submissions. Moderate novelty bar.

**Goal 2 — Grand Challenges:** Highly realistic drug-development scenarios. High novelty bar and deeper scientific review. A publication pathway with *Quantitative Medicine* is being explored.

All benchmarks must:

- ✅ Be **pharmacometric in nature** (PK, PD, exposure-response, or related)
- ✅ Be **well documented** (generative process or scenario description, yspec YAML data dictionary)
- ✅ Have **associated tasks** with defined metrics
- ✅ Have a **specified train/test split**
- ✅ Include a **motivation section** (why this dataset, what's similar, what's different)

## 🤝 Contributing

We welcome contributions! Please see:

- [Scope & Eligibility](https://aiml-sig.github.io/pmx_benchmarks/scope.html)
- [Submission Guide](https://aiml-sig.github.io/pmx_benchmarks/submission-guide.html)
- [Pull Request Template](.github/PULL_REQUEST_TEMPLATE.md)

## 📝 License

The MIT License applies to code, documentation, and benchmark data. When redistributing them, retain the copyright and license notice. We also ask that you cite the benchmarks you use. A DOI is planned for accepted submissions; the current format example has no DOI.

## 📧 Contact

- **Issues:** [Report an issue or ask a question](https://github.com/AIML-SIG/pmx_benchmarks/issues)
- **Contact page:** [aiml-sig.github.io/pmx_benchmarks/contact.html](https://aiml-sig.github.io/pmx_benchmarks/contact.html)

## 🏛️ Governance

The initiative is being developed by the AI/ML SIG Benchmarking Datasets Working Group, with hosting under the International Society of Pharmacometrics (ISoP) planned.

For more information, see our [About page](https://aiml-sig.github.io/pmx_benchmarks/about.html).
