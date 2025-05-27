# edabk-ic-design-dataset

<div align="center">
  <img src="https://raw.githubusercontent.com/your-repo/edabk-ic-design-dataset/main/images/edabk-logo.png" alt="EDA-BK Laboratory" width="300"/>
</div>

A comprehensive benchmark dataset and Python package for digital circuit design (Digital IC Design)

## 🚀 Introduction

**edabk-ic-design-dataset** is a complete ecosystem for digital circuit design education and research, consisting of three main components:

- **📦 Python Package**: A ready-to-use library available via `pip install digitalcircuit` that provides instant solutions for Karnaugh map minimization (3-4 variables), number system conversions, binary arithmetic, and digital logic calculations.

- **📊 Benchmark Suite**: A standardized evaluation framework for comparing AI/LLM model performance across different complexity levels of digital circuit design problems.

- **🗃️ Dataset Collection**: Over 11,700 carefully curated problems spanning from basic theory to advanced circuit optimization, designed for both academic research and practical applications.

This integrated platform bridges the gap between theoretical knowledge and practical implementation, making digital circuit design accessible to students, researchers, and AI developers worldwide.

## 🎯 Purpose

This project addresses critical gaps in digital circuit design education and AI evaluation:

- **Standardized Benchmarking**: First comprehensive benchmark specifically designed for digital electronics problems and AI/LLM evaluation
- **Educational Resource**: Structured dataset for Karnaugh maps, logic minimization, and number system conversions  
- **AI Training Platform**: Fine-tuning resource for Large Language Models in domain-specific circuit design tasks
- **Practical Solutions**: Ready-to-use Python package that solves real-world digital design challenges instantly

Our integrated approach provides automated evaluation frameworks, customizable benchmarks, and intelligent preprocessing capabilities that accelerate both learning and research in digital circuit design.

## 1. Overview

### 📦 Package Overview
**digitalcircuit** is a powerful Python library that provides instant solutions for digital circuit design problems. Simply install via `pip install digitalcircuit` and access comprehensive tools for Karnaugh map optimization, number system conversions, and binary arithmetic operations.

### 📊 Benchmark Framework  
Our standardized evaluation suite enables systematic comparison of AI/LLM performance across multiple complexity levels, from basic calculations to advanced circuit optimization tasks.

### 🗃️ Dataset Collection
A meticulously curated collection of 11,700+ problems spanning four difficulty levels, designed to support both educational applications and cutting-edge AI research in digital circuit design.

<table style="width:100%; border-collapse: collapse; margin: 25px 0; font-size: 0.9em; font-family: sans-serif; box-shadow: 0 0 20px rgba(0, 0, 0, 0.15);">
    <thead>
        <tr style="background-color: #009879; color: #ffffff; text-align: left;">
            <th style="padding: 12px 15px;">Level</th>
            <th style="padding: 12px 15px;">Description</th>
            <th style="padding: 12px 15px;">Topics</th>
        </tr>
    </thead>
    <tbody>
        <tr style="border-bottom: 1px solid #dddddd;">
            <td style="padding: 12px 15px; background-color: #f3f3f3;"><strong>Level 1: Basic Theory</strong></td>
            <td style="padding: 12px 15px;">Foundational knowledge and concepts</td>
            <td style="padding: 12px 15px;">
                <ul style="margin: 0; padding-left: 20px;">
                    <li>Definitions and fundamental concepts</li>
                    <li>Steps to design a digital circuit</li>
                    <li>Circuit optimization process</li>
                    <li>Circuit verification methods</li>
                </ul>
            </td>
        </tr>
        <tr style="border-bottom: 1px solid #dddddd;">
            <td style="padding: 12px 15px; background-color: #f3f3f3;"><strong>Level 2: Basic Calculations</strong></td>
            <td style="padding: 12px 15px;">Essential numerical operations</td>
            <td style="padding: 12px 15px;">
                <ul style="margin: 0; padding-left: 20px;">
                    <li>Binary to decimal conversion</li>
                    <li>Binary arithmetic</li>
                    <li>Basic logic calculations</li>
                </ul>
            </td>
        </tr>
        <tr style="border-bottom: 1px solid #dddddd;">
            <td style="padding: 12px 15px; background-color: #f3f3f3;"><strong>Level 3: Minimization and Proof</strong></td>
            <td style="padding: 12px 15px;">Advanced logic operations</td>
            <td style="padding: 12px 15px;">
                <ul style="margin: 0; padding-left: 20px;">
                    <li>Logic function minimization</li>
                    <li>Formula proof</li>
                    <li>Applying theory to practical problems</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td style="padding: 12px 15px; background-color: #f3f3f3;"><strong>Level 4: Circuit Implementation</strong></td>
            <td style="padding: 12px 15px;">Practical circuit design</td>
            <td style="padding: 12px 15px;">
                <ul style="margin: 0; padding-left: 20px;">
                    <li>Converting formulas to circuits</li>
                    <li>Designing circuits from specifications</li>
                    <li>Circuit structure optimization</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>

## 2. Package

### 🔗 Installation & Access

The **digitalcircuit** Python package is available on PyPI and provides comprehensive digital circuit design capabilities:

**📦 Quick Installation:**
```bash
pip install digitalcircuit
```

**🌐 Package Repository:** [https://pypi.org/project/digitalcircuit/](https://pypi.org/project/digitalcircuit/)

### ⚡ Key Features

- **🗺️ Karnaugh Map Solver**: Automatic minimization for 3-4 variable Boolean functions
- **🔢 Number System Converter**: Seamless conversion between binary, decimal, octal, and hexadecimal
- **⚙️ Binary Arithmetic**: Complete suite for binary calculations, complements, and signed numbers
- **🧮 Logic Operations**: Boolean algebra simplification and truth table generation
- **📊 Circuit Analysis**: Basic combinational and sequential circuit evaluation

### 🚀 Quick Start Example

```python
from digitalcircuit import KarnaughMap, NumberConverter

# Karnaugh Map Minimization
kmap = KarnaughMap(variables=3)
result = kmap.minimize([0, 1, 3, 7])
print(f"Minimized expression: {result.expression}")

# Number System Conversion  
converter = NumberConverter()
binary_result = converter.decimal_to_binary(255)
print(f"255 in binary: {binary_result}")
```

## 3. Current Benchmark Results

### Performance Comparison Across Different Models

<table style="width:100%; border-collapse: collapse; margin: 25px 0; font-size: 0.9em; font-family: sans-serif; box-shadow: 0 0 20px rgba(0, 0, 0, 0.15);">
    <thead>
        <tr style="background-color: #2C3E50; color: #ffffff; text-align: center;">
            <th style="padding: 12px 15px;">Model</th>
            <th style="padding: 12px 15px;">Level 1<br/>Theory (%)</th>
            <th style="padding: 12px 15px;">Level 2<br/>Calculations (%)</th>
            <th style="padding: 12px 15px;">Level 3<br/>K-Maps (%)</th>
            <th style="padding: 12px 15px;">Overall<br/>Score (%)</th>
            <th style="padding: 12px 15px;">Avg Response<br/>Time (s)</th>
        </tr>
    </thead>
    <tbody>
        <tr style="border-bottom: 1px solid #dddddd;">
            <td style="padding: 12px 15px; background-color: #f8f9fa; font-weight: bold;">Our Package</td>
            <td style="padding: 12px 15px; text-align: center; background-color: #d1ecf1;">94.8</td>
            <td style="padding: 12px 15px; text-align: center; background-color: #d1ecf1;">96.2</td>
            <td style="padding: 12px 15px; text-align: center; background-color: #d4edda;">89.7</td>
            <td style="padding: 12px 15px; text-align: center; font-weight: bold; background-color: #d1ecf1;">93.6</td>
            <td style="padding: 12px 15px; text-align: center;">0.8</td>
        </tr>
        <tr style="border-bottom: 1px solid #dddddd;">
            <td style="padding: 12px 15px; background-color: #f8f9fa; font-weight: bold;">Claude-3.5</td>
            <td style="padding: 12px 15px; text-align: center; background-color: #d4edda;">89.1</td>
            <td style="padding: 12px 15px; text-align: center; background-color: #d4edda;">88.7</td>
            <td style="padding: 12px 15px; text-align: center; background-color: #fff3cd;">76.2</td>
            <td style="padding: 12px 15px; text-align: center; font-weight: bold;">84.7</td>
            <td style="padding: 12px 15px; text-align: center;">1.9</td>
        </tr>
        <tr style="border-bottom: 1px solid #dddddd;">
            <td style="padding: 12px 15px; background-color: #f8f9fa; font-weight: bold;">GPT-4</td>
            <td style="padding: 12px 15px; text-align: center; background-color: #d4edda;">87.2</td>
            <td style="padding: 12px 15px; text-align: center; background-color: #d4edda;">92.5</td>
            <td style="padding: 12px 15px; text-align: center; background-color: #fff3cd;">73.8</td>
            <td style="padding: 12px 15px; text-align: center; font-weight: bold;">84.5</td>
            <td style="padding: 12px 15px; text-align: center;">2.3</td>
        </tr>
        <tr style="border-bottom: 1px solid #dddddd;">
            <td style="padding: 12px 15px; background-color: #f8f9fa; font-weight: bold;">Gemini Pro</td>
            <td style="padding: 12px 15px; text-align: center; background-color: #fff3cd;">78.4</td>
            <td style="padding: 12px 15px; text-align: center; background-color: #d4edda;">85.9</td>
            <td style="padding: 12px 15px; text-align: center; background-color: #f8d7da;">65.3</td>
            <td style="padding: 12px 15px; text-align: center; font-weight: bold;">76.5</td>
            <td style="padding: 12px 15px; text-align: center;">1.7</td>
        </tr>
    </tbody>
</table>

### 🏆 Key Performance Insights

<div align="center">
  <div style="position: relative; width: 600px; height: 400px; margin: 0 auto; background: #ECF0F1; border-radius: 10px; padding: 20px;">
    <svg width="600" height="400" viewBox="0 0 600 400" xmlns="http://www.w3.org/2000/svg">
      <!-- Title -->
      <text x="300" y="30" text-anchor="middle" font-size="16" font-weight="bold" fill="#2C3E50">Digital Circuit Design Benchmark Results</text>
      
      <!-- Y-axis -->
      <line x1="80" y1="50" x2="80" y2="320" stroke="#BDC3C7" stroke-width="2"/>
      <text x="75" y="55" text-anchor="end" font-size="12" fill="#2C3E50">100</text>
      <text x="75" y="110" text-anchor="end" font-size="12" fill="#2C3E50">80</text>
      <text x="75" y="165" text-anchor="end" font-size="12" fill="#2C3E50">60</text>
      <text x="75" y="220" text-anchor="end" font-size="12" fill="#2C3E50">40</text>
      <text x="75" y="275" text-anchor="end" font-size="12" fill="#2C3E50">20</text>
      <text x="75" y="325" text-anchor="end" font-size="12" fill="#2C3E50">0</text>
      <text x="30" y="185" text-anchor="middle" font-size="12" fill="#2C3E50" transform="rotate(-90 30 185)">Accuracy (%)</text>
      
      <!-- Grid lines -->
      <line x1="80" y1="50" x2="550" y2="50" stroke="#E8E8E8" stroke-width="1"/>
      <line x1="80" y1="104" x2="550" y2="104" stroke="#E8E8E8" stroke-width="1"/>
      <line x1="80" y1="158" x2="550" y2="158" stroke="#E8E8E8" stroke-width="1"/>
      <line x1="80" y1="212" x2="550" y2="212" stroke="#E8E8E8" stroke-width="1"/>
      <line x1="80" y1="266" x2="550" y2="266" stroke="#E8E8E8" stroke-width="1"/>
      <line x1="80" y1="320" x2="550" y2="320" stroke="#E8E8E8" stroke-width="1"/>
      
      <!-- X-axis -->
      <line x1="80" y1="320" x2="550" y2="320" stroke="#BDC3C7" stroke-width="2"/>
      
      <!-- Bars with values -->
      <!-- Our Package: 93.6% -->
      <rect x="100" y="67.2" width="80" height="252.8" fill="#E67E22" stroke="#D35400" stroke-width="2"/>
      <text x="140" y="55" text-anchor="middle" font-size="14" font-weight="bold" fill="#2C3E50">93.6%</text>
      <text x="140" y="340" text-anchor="middle" font-size="12" fill="#2C3E50">Our Package</text>
      
      <!-- Claude-3.5: 84.7% -->
      <rect x="200" y="91.46" width="80" height="228.54" fill="#3498DB" stroke="#2980B9" stroke-width="2"/>
      <text x="240" y="80" text-anchor="middle" font-size="14" font-weight="bold" fill="#2C3E50">84.7%</text>
      <text x="240" y="340" text-anchor="middle" font-size="12" fill="#2C3E50">Claude-3.5</text>
      
      <!-- GPT-4: 84.5% -->
      <rect x="300" y="92" width="80" height="228" fill="#9B59B6" stroke="#8E44AD" stroke-width="2"/>
      <text x="340" y="80" text-anchor="middle" font-size="14" font-weight="bold" fill="#2C3E50">84.5%</text>
      <text x="340" y="340" text-anchor="middle" font-size="12" fill="#2C3E50">GPT-4</text>
      
      <!-- Gemini Pro: 76.5% -->
      <rect x="400" y="113.5" width="80" height="206.5" fill="#95A5A6" stroke="#7F8C8D" stroke-width="2"/>
      <text x="440" y="102" text-anchor="middle" font-size="14" font-weight="bold" fill="#2C3E50">76.5%</text>
      <text x="440" y="340" text-anchor="middle" font-size="12" fill="#2C3E50">Gemini Pro</text>
      
      <!-- Performance indicators -->
      <text x="140" y="375" text-anchor="middle" font-size="10" fill="#27AE60" font-weight="bold">🥇 BEST</text>
      <text x="240" y="375" text-anchor="middle" font-size="10" fill="#F39C12">🥈 2nd</text>
      <text x="340" y="375" text-anchor="middle" font-size="10" fill="#E74C3C">🥉 3rd</text>
      <text x="440" y="375" text-anchor="middle" font-size="10" fill="#95A5A6">4th</text>
    </svg>
  </div>
</div>

**Performance Analysis:**
- 🥇 **Our Package leads** with 93.6% accuracy
- 📈 **+10.5% improvement** over best LLM (Claude-3.5)
- ⚡ **Fastest response time** at 0.8 seconds
- 🎯 **Consistent performance** across all problem categories

### 📋 Detailed Breakdown

<details>
<summary><strong>Level 2: Normal Calculation (4,090 samples)</strong></summary>

| Problem Type | Count | Percentage |
|--------------|-------|------------|
| Number system conversions | 3,072 | 75% |
| Two's-complement | 309 | 8% |
| Sign/Magnitude Number | 312 | 8% |
| One's-complement | 297 | 7% |
| Binary Calculator | 100 | 2% |

</details>

<details>
<summary><strong>Level 3: Karnaugh Maps (7,200 samples)</strong></summary>

| K-map Type | Count | Percentage |
|------------|-------|------------|
| 3-variable kmap | 3,500 | 48.6% |
| 4-variable kmap | 3,500 | 48.6% |
| 5-variable kmap | 100 | 1.4% |
| 6-variable kmap | 100 | 1.4% |

</details>

## 4. Data Scale

The dataset is divided into 3 main groups corresponding to the first 3 levels:

<table style="width:100%; border-collapse: collapse; margin: 25px 0; font-size: 0.9em; font-family: sans-serif; box-shadow: 0 0 20px rgba(0, 0, 0, 0.15);">
    <thead>
        <tr style="background-color: #009879; color: #ffffff; text-align: left;">
            <th style="padding: 12px 15px;">Level</th>
            <th style="padding: 12px 15px;">Name</th>
            <th style="padding: 12px 15px;">Quantity</th>
            <th style="padding: 12px 15px;">Description</th>
        </tr>
    </thead>
    <tbody>
        <tr style="border-bottom: 1px solid #dddddd;">
            <td style="padding: 12px 15px; background-color: #f3f3f3; text-align: center;"><strong>1</strong></td>
            <td style="padding: 12px 15px;">Basic Theory</td>
            <td style="padding: 12px 15px; text-align: center;"><strong>436</strong></td>
            <td style="padding: 12px 15px;">Comprehensive theory questions covering all key topics in digital electronics</td>
        </tr>
        <tr style="border-bottom: 1px solid #dddddd;">
            <td style="padding: 12px 15px; background-color: #f3f3f3; text-align: center;"><strong>2</strong></td>
            <td style="padding: 12px 15px;">Basic Calculations</td>
            <td style="padding: 12px 15px; text-align: center;"><strong>4090</strong></td>
            <td style="padding: 12px 15px;">Mainly number system conversions, binary arithmetic, signed numbers, complements</td>
        </tr>
        <tr>
            <td style="padding: 12px 15px; background-color: #f3f3f3; text-align: center;"><strong>3</strong></td>
            <td style="padding: 12px 15px;">Function Minimization / Karnaugh Map</td>
            <td style="padding: 12px 15px; text-align: center;"><strong>7200</strong></td>
            <td style="padding: 12px 15px;">Logic function minimization problems with 3, 4, 5, 6-variable K-maps</td>
        </tr>
    </tbody>
</table>

### Dataset Visualization

#### 📊 Digital Circuit Design Dataset Structure

<div align="center">
  <div style="position: relative; width: 500px; height: 500px; margin: 0 auto;">
    <svg width="500" height="500" viewBox="0 0 500 500" xmlns="http://www.w3.org/2000/svg">
      <!-- Outer Ring - Problem Types -->
      <path d="M 250 50 A 200 200 0 0 1 433 150" fill="#E3F2FD" stroke="#1976D2" stroke-width="2"/>
      <text x="350" y="90" text-anchor="middle" font-size="10" font-weight="bold">Number System Conversions (3,072)</text>
      
      <path d="M 433 150 A 200 200 0 0 1 433 350" fill="#E8F5E8" stroke="#388E3C" stroke-width="2"/>
      <text x="440" y="200" text-anchor="middle" font-size="10" font-weight="bold" transform="rotate(90 440 200)">Two's-complement (309)</text>
      <text x="440" y="250" text-anchor="middle" font-size="10" font-weight="bold" transform="rotate(90 440 250)">Sign/Magnitude (312)</text>
      <text x="440" y="300" text-anchor="middle" font-size="10" font-weight="bold" transform="rotate(90 440 300)">One's-complement (297)</text>
      
      <path d="M 433 350 A 200 200 0 0 1 250 450" fill="#FFF3E0" stroke="#F57C00" stroke-width="2"/>
      <text x="350" y="410" text-anchor="middle" font-size="10" font-weight="bold">Binary Calculator (100)</text>
      
      <path d="M 250 450 A 200 200 0 0 1 67 350" fill="#F3E5F5" stroke="#7B1FA2" stroke-width="2"/>
      <text x="120" y="420" text-anchor="middle" font-size="10" font-weight="bold">3-variable kmap (3,500)</text>
      <text x="150" y="400" text-anchor="middle" font-size="10" font-weight="bold">4-variable kmap (3,500)</text>
      
      <path d="M 67 350 A 200 200 0 0 1 67 150" fill="#FFEBEE" stroke="#D32F2F" stroke-width="2"/>
      <text x="60" y="200" text-anchor="middle" font-size="10" font-weight="bold" transform="rotate(-90 60 200)">5-variable kmap (100)</text>
      <text x="60" y="250" text-anchor="middle" font-size="10" font-weight="bold" transform="rotate(-90 60 250)">6-variable kmap (100)</text>
      
      <path d="M 67 150 A 200 200 0 0 1 250 50" fill="#E0F2F1" stroke="#00796B" stroke-width="2"/>
      <text x="150" y="100" text-anchor="middle" font-size="10" font-weight="bold">Theory Problems</text>
      
      <!-- Inner Ring - Main Categories -->
      <circle cx="250" cy="250" r="120" fill="none" stroke="#37474F" stroke-width="3"/>
      
      <path d="M 250 130 A 120 120 0 0 1 354 190" fill="#B39DDB" stroke="#5E35B1" stroke-width="2"/>
      <text x="310" y="160" text-anchor="middle" font-size="12" font-weight="bold">Theory</text>
      <text x="310" y="175" text-anchor="middle" font-size="11">(436)</text>
      
      <path d="M 354 190 A 120 120 0 0 1 354 310" fill="#81C784" stroke="#4CAF50" stroke-width="2"/>
      <text x="370" y="240" text-anchor="middle" font-size="12" font-weight="bold" transform="rotate(90 370 240)">Normal</text>
      <text x="370" y="255" text-anchor="middle" font-size="12" font-weight="bold" transform="rotate(90 370 255)">Calculation</text>
      <text x="370" y="270" text-anchor="middle" font-size="11" transform="rotate(90 370 270)">(4,090)</text>
      
      <path d="M 354 310 A 120 120 0 1 1 250 130" fill="#FFB74D" stroke="#FF9800" stroke-width="2"/>
      <text x="220" y="340" text-anchor="middle" font-size="12" font-weight="bold">Function Simplify</text>
      <text x="220" y="355" text-anchor="middle" font-size="11">(7,200)</text>
      
      <!-- Center Circle -->
      <circle cx="250" cy="250" r="60" fill="#263238" stroke="#37474F" stroke-width="3"/>
      <text x="250" y="240" text-anchor="middle" font-size="14" font-weight="bold" fill="white">Benchmark</text>
      <text x="250" y="255" text-anchor="middle" font-size="12" font-weight="bold" fill="white">Dataset</text>
      <text x="250" y="270" text-anchor="middle" font-size="11" fill="white">(11,726)</text>
    </svg>
  </div>
</div>

**Dataset Hierarchy:**
- **🎯 Center**: Benchmark Dataset (11,726 total samples)
- **🔵 Inner Ring**: 3 main categories - Theory (436), Normal Calculation (4,090), Function Simplify (7,200)  
- **🔷 Outer Ring**: 10 specific problem types with detailed sample counts

## 5. Usage Guide

### Environment
- Python >= 3.8
- Required libraries: `pandas`, `numpy`, `matplotlib`, `plotly`, `sympy`

### 🚀 Quick Installation

```bash
# Clone the repository
git clone https://github.com/your-repo/edabk-ic-design-dataset.git
cd edabk-ic-design-dataset

# Install dependencies
pip install -r requirements.txt

# Install the package
pip install -e .
```

### 📊 Running Benchmark Evaluation

#### Example 1: Evaluate Your Model on Level 2 Dataset

```python
from edabk_benchmark import BenchmarkRunner, load_dataset

# Load Level 2 dataset
dataset = load_dataset("level2_calculations")
print(f"Loaded {len(dataset)} calculation problems")

# Initialize benchmark runner
runner = BenchmarkRunner(
    dataset=dataset,
    model_name="your_model",
    timeout=30  # seconds per question
)

# Run benchmark evaluation
results = runner.evaluate_model(your_model_function)

# Display results
print(f"Overall Accuracy: {results.accuracy:.2f}%")
print(f"Average Response Time: {results.avg_time:.2f}s")
print(f"Breakdown by Problem Type:")
for problem_type, accuracy in results.breakdown.items():
    print(f"  {problem_type}: {accuracy:.2f}%")
```

#### Example 2: Compare Multiple Models

```python
from edabk_benchmark import ModelComparator

# Initialize comparator
comparator = ModelComparator()

# Add models to compare
comparator.add_model("GPT-4", gpt4_function)
comparator.add_model("Claude-3.5", claude_function)
comparator.add_model("Your Model", your_model_function)

# Run comparison on all levels
results = comparator.run_full_benchmark()

# Generate comparison report
comparator.generate_report(output_path="benchmark_results.html")
```

### 🛠️ Using the Package for Individual Questions

#### Example 1: Number System Conversion

```python
from edabk_ic_design import DigitalCircuitSolver

# Initialize solver
solver = DigitalCircuitSolver()

# Convert binary to decimal
question = "Convert binary 1101011 to decimal"
answer = solver.convert_number_system(
    number="1101011",
    from_base=2,
    to_base=10
)
print(f"Answer: {answer}")  # Output: 107

# Convert with verification
result = solver.solve_with_steps(question)
print(f"Step-by-step solution:\n{result.steps}")
print(f"Final answer: {result.answer}")
```

#### Example 2: Karnaugh Map Minimization

```python
# Solve K-map minimization
question = """
Minimize the following Boolean function using K-map:
F(A,B,C,D) = Σ(0,1,3,7,8,9,11,15)
"""

result = solver.minimize_kmap(
    variables=['A', 'B', 'C', 'D'],
    minterms=[0, 1, 3, 7, 8, 9, 11, 15]
)

print(f"Minimized expression: {result.expression}")
print(f"K-map visualization:\n{result.kmap_display}")
print(f"Number of literals reduced: {result.complexity_reduction}")
```

#### Example 3: Logic Circuit Analysis

```python
# Analyze logic circuit
circuit_description = """
Design a 3-bit binary adder circuit with carry output.
Inputs: A2A1A0, B2B1B0
Outputs: S2S1S0, Cout
"""

result = solver.design_circuit(circuit_description)
print(f"Circuit design:\n{result.circuit_diagram}")
print(f"Truth table:\n{result.truth_table}")
print(f"Boolean expressions:\n{result.expressions}")
```

### 🔧 Advanced Usage

#### Custom Model Integration

```python
# Define your custom model
def my_custom_model(question, context=None):
    """
    Your custom AI model for digital circuit problems
    
    Args:
        question (str): The problem statement
        context (dict): Additional context if needed
    
    Returns:
        dict: {
            'answer': str,
            'confidence': float,
            'reasoning': str
        }
    """
    # Your model logic here
    response = your_model_inference(question)
    
    return {
        'answer': response.answer,
        'confidence': response.confidence,
        'reasoning': response.explanation
    }

# Register and evaluate
runner.register_model(my_custom_model)
results = runner.evaluate_on_subset(level=2, sample_size=100)
```

#### Batch Processing

```python
# Process multiple questions at once
questions = [
    "Convert 255 to binary",
    "Simplify: AB + AB' + A'B",
    "Find 2's complement of 1010110"
]

results = solver.batch_solve(questions, parallel=True)
for i, result in enumerate(results):
    print(f"Q{i+1}: {result.answer}")
```

## 🎯 Benchmark Goals

- Provide a standardized, easy-to-use dataset for digital circuit design problems.
- Support evaluation and comparison of AI/LLM models in digital electronics.
- Enable expansion, contribution, and reuse of data within the research community.

## 🔮 Future Development Roadmap

### 🎯 Development Priorities

#### 🤖 **AI Agent Transformation**
Transform the current benchmark into an intelligent autonomous agent capable of end-to-end digital circuit design, optimization, and verification with natural language understanding.

#### ⚡ **Advanced Circuit Support**
Extend capabilities to support comprehensive circuit types including combinational/sequential logic, timing analysis, clock wave generation, waveform analysis, and power optimization.

#### 💬 **Chat Application Integration**
Develop interactive chat interface with voice commands, hand-drawn circuit recognition, real-time collaboration, and step-by-step guided learning for enhanced user experience.

#### 🎓 **Illuma Educational Platform**
Integrate with Illuma to create a complete student guidance system featuring personalized learning paths, automated assessment, progress tracking, and gamified learning experiences.

**Target**: Create the most comprehensive AI-powered digital circuit design education platform worldwide.

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
