# edabk-ic-design-dataset

A benchmark dataset for digital circuit design (Digital IC Design)

## 1. Overview of the Benchmark

The benchmark is divided into 4 levels from basic to advanced:

### Level 1: Basic Theory
- Definitions and fundamental concepts
  + Number systems (binary, decimal, hexadecimal)
  + Boolean algebra and logic operations
  + Basic logic gates (AND, OR, NOT, NAND, NOR, XOR)
  + Truth tables and logic expressions
  + Minterm and Maxterm
  + Karnaugh Map (K-map)
  + Combinational and sequential circuits
  + Flip-flops and memory types
  + Encoding and decoding
  + Multiplexer and Demultiplexer
  + Adders and subtractors
  + Comparators
  + Counters and frequency dividers
  + Circuit optimization methods
  + Design and verification standards
  + IC fabrication technologies (CMOS, TTL, ECL)
  + Key technical parameters (speed, power, noise)
  + Testing and debugging methods
  + Design and simulation tools
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

### Data quantity and classification

The dataset is divided into 3 main groups corresponding to the first 3 levels:

| Level | Name | Quantity | Description |
|-------|------|----------|-------------|
| 1 | Basic Theory | 436 | Comprehensive theory questions covering all key topics in digital electronics |
| 2 | Basic Calculations | 4090 | Mainly number system conversions, binary arithmetic, signed numbers, complements, ... |
| 3 | Function Minimization / Karnaugh Map | 7200 | Logic function minimization problems with 3, 4, 5, 6-variable K-maps |

#### Detailed statistics:
- **Level 1:** 436 theory questions (crawled and manually verified)
- **Level 2:** 4090 problems, including:
  - 3072 number system conversions (75%)
  - 100 binary calculator (2%)
  - 312 sign/magnitude numbers (8%)
  - 297 one's-complement (7%)
  - 309 two's-complement (8%)
- **Level 3:** 7200 K-map problems, including:
  - 3500 3-variable K-map (49%)
  - 3500 4-variable K-map (49%)
  - 100 5-variable K-map (1%)
  - 100 6-variable K-map (1%)

#### Data construction methods
- Level 1: Data crawling + manual verification
- Level 2: Tool + real exercises
- Level 3: Automatic tool generation

#### Token statistics
- Level 1: 21,695
- Level 2: 1,204,064
- Level 3: 3,192,868

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





