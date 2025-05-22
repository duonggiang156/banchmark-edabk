# edabk-ic-design-dataset

A benchmark dataset for digital circuit design (Digital IC Design)

## 🔍 Purpose of the Dataset

This dataset was created to address critical gaps in the field of digital circuit design:

- Currently, there is no specific benchmark for digital electronics design problems, especially for AI/LLM models.
- There is a lack of standardized datasets for Karnaugh maps and logic function minimization techniques.
- Standardized datasets for number system conversions and calculations in different numerical systems are missing.
- There is a need for a platform to evaluate AI model performance in solving digital circuit design problems.

This dataset aims to fill these gaps by providing a comprehensive and diverse collection of data for both academic research and industrial applications.

## 1. Overview of the Benchmark

The benchmark is designed with progressive levels from basic to advanced, allowing users to approach concepts gradually and comprehensively.

| Level | Module Name | Key Content | Skills Developed |
|--------|------------|----------------|-------------------|
| **Level 1** | Basic Theory | • Fundamental concepts (number systems, Boolean algebra)<br>• Logic gates, truth tables, K-maps<br>• Digital circuit design process<br>• Circuit optimization methods | Understanding and applying basic concepts |
| **Level 2** | Basic Calculations | • Conversions between number systems (binary, decimal, etc.)<br>• Binary arithmetic<br>• Basic logic calculations | Performing calculations and conversions |
| **Level 3** | Minimization and Proof | • Logic function minimization<br>• Formula proof<br>• Applying theory to practical problems | Analyzing and optimizing logic circuits |
| **Level 4** | Circuit Implementation | • Converting formulas to circuits<br>• Designing circuits from specifications<br>• Optimizing circuit structures | Designing and implementing complete digital circuits |

## 2. Dataset Scale

The dataset is divided into 3 main groups corresponding to the first 3 levels:

| Level | Name | Quantity | Description |
|-------|------|----------|-------------|
| 1 | Basic Theory | 436 | Comprehensive theory questions covering all key topics in digital electronics |
| 2 | Basic Calculations | 4090 | Mainly number system conversions, binary arithmetic, signed numbers, complements, ... |
| 3 | Function Minimization / Karnaugh Map | 7200 | Logic function minimization problems with 3, 4, 5, 6-variable K-maps |

### Dataset visualization

Dưới đây là code để tạo lại biểu đồ thống kê dữ liệu:

```python
import matplotlib.pyplot as plt
import numpy as np

# Code để tạo biểu đồ tổng dữ liệu
def plot_total_data():
    categories = ['Function simplify\n(Tool)', 'Normal Calculation\n(Tool + Exercise)', 'Theory\n(Crawl data tool + Human verify)']
    values = [7200, 4090, 436]
    colors = ['#ff0000', '#ffff00', '#00aa44']
    
    fig, ax = plt.subplots(figsize=(10, 6))
    bars = ax.barh(categories, values, color=colors)
    
    # Thêm giá trị vào cuối mỗi thanh
    for bar in bars:
        width = bar.get_width()
        ax.text(width + 50, bar.get_y() + bar.get_height()/2, 
                f'{int(width)}', ha='left', va='center')
    
    ax.set_title('Total Data', fontsize=18, color='#ff0000', fontweight='bold')
    ax.set_xlim(0, 8000)
    ax.grid(axis='x', linestyle='-', alpha=0.3)
    ax.spines['top'].set_visible(False)
    ax.spines['right'].set_visible(False)
    
    plt.tight_layout()
    plt.savefig('images/total_data_visualization.png', dpi=300, bbox_inches='tight')
    plt.show()

# Code để tạo biểu đồ Karnaugh Maps level 3
def plot_kmap_distribution():
    labels = ['3-variable kmap', '4-variable kmap', '5-variable kmap', '6-variable kmap']
    sizes = [49, 49, 1, 1]  # Phần trăm
    colors = ['#ff7700', '#0099cc', '#00aa44', '#cc5500']
    
    fig, ax = plt.subplots(figsize=(8, 6))
    ax.pie(sizes, colors=colors, startangle=90, 
           wedgeprops={'edgecolor': 'white', 'linewidth': 1, 'antialiased': True})
    
    # Thêm chú thích với ô màu nền
    for i, label in enumerate(labels):
        percentage = f'{sizes[i]}%'
        x_offset = 0.7 if i < 2 else 0.6
        y_offset = 0.2 if i == 0 else -0.2 if i == 1 else 0.1 if i == 2 else -0.1
        
        plt.annotate(
            label, 
            xy=(x_offset, y_offset),
            xytext=(1.1, 0),
            textcoords='axes fraction',
            bbox=dict(boxstyle="round,pad=0.3", fc="white", ec="black", lw=1),
            ha='left', va='center'
        )
        
        # Thêm % vào biểu đồ
        if sizes[i] > 2:  # Chỉ hiển thị % cho phần có kích thước đủ lớn
            plt.annotate(
                f'{sizes[i]}%',
                xy=(x_offset, y_offset),
                ha='center', va='center',
                fontsize=12, fontweight='bold'
            )
    
    ax.set_title('Karnaugh Maps - level 3', fontsize=18, color='#ff0000', fontweight='bold')
    plt.tight_layout()
    plt.savefig('images/kmap_distribution.png', dpi=300, bbox_inches='tight')
    plt.show()

# Code để tạo biểu đồ Normal Calculation level 2
def plot_calculation_distribution():
    labels = ['Number system conversions', 'Sign/Magnitude Number', 'Binary Calculator', 
              "One's-complement", "Two's-complement"]
    sizes = [75, 8, 7, 8, 2]  # Phần trăm
    colors = ['#0099cc', '#00aa44', '#aa5500', '#884400', '#005588']
    
    fig, ax = plt.subplots(figsize=(8, 6))
    ax.pie(sizes, colors=colors, startangle=90, 
           wedgeprops={'edgecolor': 'white', 'linewidth': 1, 'antialiased': True})
    
    # Thêm % vào biểu đồ
    for i, p in enumerate(sizes):
        ang = 2 * np.pi * (sum(sizes[:i]) + p/2) / sum(sizes)
        x = 0.7 * np.cos(ang)
        y = 0.7 * np.sin(ang)
        if p > 5:  # Chỉ hiển thị % cho phần có kích thước đủ lớn
            ax.annotate(f'{p}%', xy=(x, y), ha='center', va='center', fontsize=12, fontweight='bold')
    
    # Tạo chú thích
    ax.legend(labels, loc='lower center', bbox_to_anchor=(0.5, -0.15), ncol=2)
    
    ax.set_title('Normal Calculation - level 2', fontsize=18, color='#ff0000', fontweight='bold')
    plt.tight_layout()
    plt.savefig('images/calculation_distribution.png', dpi=300, bbox_inches='tight')
    plt.show()

# Để vẽ các biểu đồ, chạy các hàm:
# plot_total_data()
# plot_kmap_distribution()
# plot_calculation_distribution()
```

![*Total data by group*](https://github.com/duonggiang156/banchmark-edabk/blob/master/images/total.jpg)

![*Distribution of problem types in Level 2*](https://github.com/duonggiang156/banchmark-edabk/blob/master/images/level2-data.jpg)

![*Distribution of problem types in Level 3*](https://github.com/duonggiang156/banchmark-edabk/blob/master/images/level3-data.jpg)

## 3. Usage Guide

### Environment
- Python >= 3.x
- Required libraries: `pandas`, `numpy`, `matplotlib`, `plotly`

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





