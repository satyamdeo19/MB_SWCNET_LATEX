# 🧠 Multi-Band SWCNet for Cross-Session MI-BCI

This repository contains the LaTeX source code for the research paper:

**"Overcoming Session Drift and Filter Blindness in Motor Imagery BCI: A Multi-Band Space-First CNN with Euclidean Alignment"**

---

## 📄 Overview

This work proposes **MB-SWCNet**, an extension of SWCNet designed to improve cross-session EEG classification by addressing:

* **Session Drift** (covariance shift across sessions)
* **Filter Blindness** (loss of frequency-specific features in broadband processing)

---

## 📂 Project Structure

```
.
├── main.tex
├── references.bib
├── figures/
│   ├── fig1.png
│   ├── fig2.png
│   └── ...
├── output.pdf
└── README.md
```

---

## ⚙️ Installation Guide (Local Setup)

### 🟢 Step 1: Install LaTeX Distribution

Install a LaTeX engine:

* Windows: Install **MiKTeX**
* Mac/Linux: Install **TeX Live**

👉 Download:

* https://miktex.org/download
* https://www.tug.org/texlive/

### Important Settings (MiKTeX)

During installation:

* Enable **"Install missing packages on-the-fly"**
* Choose: **Yes / Always**

---

### 🟣 Step 2: Install LaTeX Editor

Install a LaTeX editor:

* Recommended: **TeXstudio**

👉 Download:

* https://www.texstudio.org/

---

### 🔵 Step 3: Verify Installation

Open TeXstudio and check:

```
Options → Configure TeXstudio → Commands
```

Ensure:

* `pdflatex` is properly configured

---

## 🚀 How to Run the Project

### Step 1: Clone the Repository

```
git clone https://github.com/YOUR_USERNAME/REPO_NAME.git
cd REPO_NAME
```

---

### Step 2: Open the Project

* Open **TeXstudio**
* Click:

  ```
  File → Open → .tex file
  ```

---

### Step 3: Compile

Press:

```
F5 (Build & View)
```

OR run in terminal:

```
pdflatex main.tex
```

---

### ⏳ First Compilation

* May take **2–5 minutes**
* MiKTeX may prompt:

  ```
  Install missing package?
  ```

  👉 Click **Install**

---

## 🖼️ Handling Figures

* All images are stored in the `figures/` directory
* Ensure this line is present in `main.tex`:

```latex
\graphicspath{{figures/}}
```

* Then images can be used as:

```latex
\includegraphics{fig1.png}
```

---

## ⚡ Fast Compile Mode (Optional)

To speed up compilation during editing:

```latex
\usepackage[draft]{graphicx}
```

This will:

* Skip loading images
* Compile much faster

---

## ❗ Common Issues & Fixes

### 1. Images Not Found

* Ensure images are in correct folder
* Check filename case (e.g., `fig1.png` vs `Fig1.png`)

---

### 2. pdflatex Not Found

* Restart TeXstudio
* Reinstall MiKTeX if needed

---

### 3. Slow Compilation

* Normal for large IEEE papers
* Use draft mode (above)

---

### 4. Missing Package Error

* Click **Install** when prompted by MiKTeX

---

## 📊 Results Summary

| Dataset    | Setup I | Setup II |
| ---------- | ------- | -------- |
| BCIC-IV-2a | 99.81%  | 74.00%   |
| HGD        | 99.96%  | 86.16%   |
| OpenBMI    | 99.50%  | 65.18%   |

---

## 📬 Contact

**Satyam Deo**
Indian Institute of Information Technology, Nagpur

---

## ⭐ If you found this useful, consider starring the repository!
