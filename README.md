# edabk-ic-design-dataset

A benchmark dataset for digital circuit design (Digital IC Design)

## 1. Overview of the Benchmark

The benchmark is divided into 4 levels from basic to advanced:

### Level 1: Basic Theory
- Definitions and fundamental concepts (number systems, Boolean algebra, logic gates, truth tables, K-maps, ...)
- Steps to design a digital circuit
- Circuit optimization process
- Circuit verification methods

### Level 2: Basic Calculations
- Binary to decimal conversion
- Binary arithmetic
- Basic logic calculations

### Level 3: Minimization and Proof
- Logic function minimization
- Formula proof
- Applying theory to practical problems

### Level 4: Circuit Implementation
- Converting formulas to circuits
- Designing circuits from specifications
- Circuit structure optimization

## 2. Dataset Scale

The dataset is divided into 3 main groups corresponding to the first 3 levels:

| Level | Name | Quantity | Description |
|-------|------|----------|-------------|
| 1 | Basic Theory | 436 | Comprehensive theory questions covering all key topics in digital electronics |
| 2 | Basic Calculations | 4090 | Mainly number system conversions, binary arithmetic, signed numbers, complements, ... |
| 3 | Function Minimization / Karnaugh Map | 7200 | Logic function minimization problems with 3, 4, 5, 6-variable K-maps |

### Dataset visualization

![*Total data by group*](https://github.com/duonggiang156/banchmark-edabk/blob/master/images/total.jpg)

![*Distribution of problem types in Level 2*](https://github.com/duonggiang156/banchmark-edabk/blob/master/images/level2-data.jpg)

![*Distribution of problem types in Level 3*](https://github.com/duonggiang156/banchmark-edabk/blob/master/images/level3-data.jpg)


## 3. Usage Guide

### Environment
- Python >= 3.x
- Required libraries: `pandas`, `numpy`, `...`

### Benchmark usage workflow

```
Step 1: Clone repository
    |
Step 2: Install dependencies
    |
Step 3: Run benchmark with the corresponding dataset
    |
Step 4: Evaluate results using metrics
```

### Detailed steps

1. **Clone repository**
   ```bash
   git clone <link-repo>
   cd <repo-folder-name>
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run benchmark**
   - Follow the instructions in the `src/` directory or use the provided notebook/scripts.

4. **Evaluate results**
   - Use the following metrics:
     - Accuracy
     - Processing time
     - Solution complexity

## 🎯 Benchmark Goals

- Provide a standardized, easy-to-use dataset for digital circuit design problems.
- Support evaluation and comparison of AI/LLM models in digital electronics.
- Enable expansion, contribution, and reuse of data within the research community.

## 🚀 Quick Start

1. Clone repository:
   ```bash
   git clone <link-repo>
   cd <repo-folder-name>
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run a sample script:
   ```bash
   python src/run_benchmark.py --dataset 1cau_convert_so.xlsx
   ```

## 🤝 Contribution & Development

- All contributions regarding data, code, or ideas are welcome!
- Please create a pull request or issue for discussion.
- To develop more benchmarks or expand the dataset, refer to the `src/` directory and contact the development team.

## 📄 Citation

If you use this dataset for research, please cite as follows:

```
@misc{edabk-ic-design-dataset,
  title={edabk-ic-design-dataset: Benchmark for digital circuit design},
  author={EDABK Development Team},
  year={2024},
  url={https://github.com/<your-repo>}
}
```





