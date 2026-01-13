# 💻 Laptop Recommendation System using SAW Method

Simple Decision Support System for recommending the best laptops based on optimal price-performance trade-off using **Simple Additive Weighting (SAW)** method.

---

## 📋 About

This project implements a Decision Support System that integrates laptop specifications with CPU and GPU benchmark data from PassMark using **fuzzy string matching**. The system ranks laptops based on four criteria with equal weighting (25% each):

- **Price (€)** - Cost criterion
- **CPU Mark** - CPU performance benchmark
- **G3D Mark** - GPU performance benchmark  
- **RAM (GB)** - Memory capacity

---

## 🗂️ Repository Contents

```
├── spk_laptop.ipynb          # Main notebook (SAW implementation)
└── dataset/
    ├── laptop.csv            # Laptop dataset from Kaggle
    ├── cpu_data.csv          # CPU benchmark from PassMark
    └── gpu_data.csv          # GPU benchmark from PassMark
```

---

## 📊 Datasets

### 1. Laptop Price Dataset
- **Source:** [Kaggle - Laptop Price Dataset](https://www.kaggle.com/datasets/ironwolf437/laptop-price-dataset)
- **License:** CC0: Public Domain

### 2. CPU & GPU Benchmarks
- **Source:** [PassMark Software](https://www.passmark.com/)
  - CPU: https://www.cpubenchmark.net/
  - GPU: https://www.videocardbenchmark.net/
- **Note:** Data for academic research purposes only

---

## 🚀 How to Use

### Prerequisites
- Python 3.12+
- Jupyter Notebook

### Required Libraries
```bash
pip install pandas numpy matplotlib seaborn
```

### Run the Notebook
1. Clone this repository
2. Open `spk_laptop.ipynb` in Jupyter
3. Run all cells to see the analysis and top 10 laptop recommendations

---

## 📈 Results Preview

The system successfully ranks laptops with **MacBook Pro** as the top recommendation (SAW score: 0.5593), followed by **Surface Laptop** (0.5310) and **Latitude 7480** (0.5299).

Full results and visualizations are available in the notebook.

---

## 🔬 Methodology

1. **Data Preprocessing:** Cleaning, normalization, and fuzzy string matching (difflib, threshold 0.7)
2. **SAW Normalization:** Benefit criteria (max norm) and cost criteria (min norm)
3. **Scoring:** Equal weighted sum (25% each criterion)
4. **Ranking:** Sort by SAW score descending

---

## 👨‍💻 Author

**Irwan Febriansyah**  
Sistem Informasi, Universitas Nahdlatul Ulama Sidoarjo  
📧 irwanfebriansyah112@gmail.com

---

## 📄 License

**Code:** Use freely for academic purposes  
**Datasets:**
- Laptop data: CC0 Public Domain (Kaggle)
- Benchmark data: PassMark Software (academic use only)

---

## 🙏 Credits

- Laptop dataset: [ironwolf437 on Kaggle](https://www.kaggle.com/datasets/ironwolf437/laptop-price-dataset)
- Benchmark data: [PassMark Software](https://www.passmark.com/)

---

**⭐ If this project helps you, please give it a star!**
