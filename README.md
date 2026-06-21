# Python Libraries
Numpy+Pandas+Matploilib

# 📊 Python Data Science – Core Libraries

A structured reference notebook series covering the three foundational Python libraries for data science: **NumPy**, **Pandas**, and **Matplotlib**. Each notebook is clean, well-commented, and designed to run top-to-bottom without errors.

---

## 📁 Repository Structure

```
📦 python-data-science/
├── README.md
├── Numpy.ipynb       # Array computing with NumPy
├── Pandas.ipynb      # Data manipulation with Pandas
└── Matplotlib.ipynb        # Data visualisation with Matplotlib
```

---

## 📓 Notebooks

### 1. `Numpy_Clean.ipynb` — Array Computing

Covers the full NumPy toolkit for fast, vectorised numerical computation.

| Section | Topics |
|---|---|
| Creating Arrays | 1-D, 2-D, 3-D arrays; `np.random` |
| Array Attributes | `ndim`, `shape`, `size`, `dtype`, `itemsize` |
| Array Indexing | Zero-based, negative indexing, modifying values |
| Array Slicing | `start:stop:step`, 2-D slicing |
| Views vs Copies | Memory sharing, `.copy()` |
| Reshaping | `reshape()`, `np.newaxis` |
| Concatenation & Stacking | `np.concatenate`, `vstack`, `hstack` |
| Splitting | `np.split`, `vsplit`, `hsplit` |
| Vectorization | Replacing loops with array operations |
| Universal Functions | Arithmetic, trig, exponential, logarithm ufuncs |
| Aggregations | `reduce`, `accumulate`, axis-wise `sum`/`min`/`max` |
| Broadcasting | Rules, feature centering, 2-D function plotting |
| Boolean Masking | Comparison operators, `any`/`all`, compound conditions |
| Fancy Indexing | Integer array indexing, `np.add.at` |
| Sorting | `sort`, `argsort`, `partition` |
| Structured Arrays | Named, typed fields in a single array |

---

### 2. `Pandas_Clean.ipynb` — Data Manipulation

Covers Pandas for loading, transforming, and analysing tabular data.

| Section | Topics |
|---|---|
| Series | Creation, custom index, from dict/scalar |
| DataFrame | From lists, dicts, NumPy arrays, structured arrays |
| Indexing & Selection | `.loc`, `.iloc`, boolean filtering, the indexing quick-reference |
| ufuncs & Alignment | Index preservation, automatic label alignment, `fill_value` |
| Missing Values | `None` vs `NaN`, `isnull`, `dropna`, `fillna`, `ffill`/`bfill` |
| Hierarchical Indexing | `MultiIndex`, `unstack`/`stack`, `sort_index`, `reset_index` |
| Combining: concat | Row/column concat, duplicate indexes, `keys`, inner/outer join |
| Combining: merge & join | One-to-one, many-to-one, many-to-many; join types; suffixes |
| Aggregation & GroupBy | `sum`, `mean`, `describe`, `groupby`, `agg` |
| Pivot Tables | `pivot_table`, multiple aggregations, `margins` |
| String Operations | `.str` accessor, regex methods, `get_dummies` |

---

### 3. `Matplotlib.ipynb` — Data Visualisation

Covers Matplotlib for creating and customising a variety of charts and plots.

| Section | Topics |
|---|---|
| Line Plots | `plot()`, line width, linestyle (`--`), markers, colour, axis labels, `yticks` |
| Scatter Plots | `scatter()`, colour (`c=`), marker style, size (`s=`) |
| Bar Charts | `bar()`, alignment, width, edge colour |
| Histograms | `hist()`, bins, cumulative distribution |
| Pie Charts | `pie()`, `explode`, `autopct`, `pctdistance`, `startangle` |
| Box Plots | `boxplot()`, normal distribution data |
| Legends | `label=`, `plt.legend()`, `loc=`, legends in pie charts |
| Multiple Lines | Plotting several series on one axes; stock comparison example |
| Multiple Figures | `plt.figure(n)` to manage independent figure windows |
| Subplots | `plt.subplots(2, 2)`, `set_title`, `suptitle`, `tight_layout` |
| Styling | `style.use()`, `dark_background`, grid with `alpha` |
| 3-D Plots | `projection='3d'`, `ax.scatter()` in three dimensions |
| Saving Figures | `savefig()`, `dpi=300`, `transparent=` |
| Practical Example | Multi-week sales report — titled axes, custom colours, real-world data |

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install numpy pandas matplotlib jupyter
```

### Running the Notebooks

```bash
# Launch Jupyter
jupyter notebook

# Or with JupyterLab
jupyter lab
```

Then open any `.ipynb` file from the file browser. Each notebook is self-contained and can be run top-to-bottom with **Kernel → Restart & Run All**.

---

## 🧠 Recommended Learning Order

```
NumPy  →  Pandas  →  Matplotlib
```

NumPy underpins both Pandas and Matplotlib. Start there, then move to data manipulation with Pandas, and finish with visualisation.

---

## 💡 Key Concepts at a Glance

| Concept | Library | Quick Example |
|---|---|---|
| Fast array math | NumPy | `arr * 2`, `np.sqrt(arr)` |
| Label-aware data | Pandas | `df.loc['Alice', 'Score']` |
| Index alignment | Pandas | `s1 + s2` aligns by label |
| Missing data | Pandas | `df.fillna(0)`, `df.dropna()` |
| Grouped summary | Pandas | `df.groupby('Dept').mean()` |
| Line chart | Matplotlib | `plt.plot(x, y, lw=2, linestyle='--')` |
| Scatter plot | Matplotlib | `plt.scatter(x, y, c='green', marker='*', s=100)` |
| Subplots | Matplotlib | `fig, axs = plt.subplots(2, 2)` |
| Save figure | Matplotlib | `plt.savefig('plot.png', dpi=300)` |

---

## 📚 References

- [NumPy Documentation](https://numpy.org/doc/)
- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Matplotlib Documentation](https://matplotlib.org/stable/index.html)
- *Python Data Science Handbook* – Jake VanderPlas (the inspiration for these notebooks)
