# CITS4012-NLP

> **NOTE**
>
> * 本`README.md`主要用于团队沟通，并在**定稿时改为English便于评分**
> * 定稿后将公开这个库，简历里能多水一行，故而**请使用 all in English commits**

## 🚀Getting Started

### Installation

```bash
git clone https://github.com/Kaichao-Zheng/CITS4012-NLP.git
```

### Create virtural environment

```bash
cd CITS4012-NLP
python -m venv venv
```

## ⚙️Setup

### Activate virtural environment

```bash
venv\Scripts\activate		# Windows PowerShell
source venv/bin/activate	# macOS/Linux
```

### Enable `.ipynb` version control using `nbstripout`

* `nbstripout`主要用于commit时自动清理`.ipynb`的输出，避免污染GitHub远程库

```bash
pip install nbstripout
nbstripout --install
```

### Enable `.ipynb` difference using `nbdime`

* 默认`git diff`显示为JSON格式，不够直观

```bash
pip install nbdime
nbdime config-git --enable
```

## 🔍Check `.ipynb` Difference

#### Option 1: Default Git Diff

```bash
git diff CITS4012_YourGroupID.ipynb
```

Press **Q** to stop.

#### Option 2: nbdime CLI Diff

```bash
nbdiff CITS4012_YourGroupID.ipynb
```

#### Option 3: nbdime GUI diff (Recommended)

![nbdime_gui](img/nbdime_gui.png)

#### Option 4: nbdime Web GUI (Recommended)

```bash
nbdiff-web CITS4012_YourGroupID.ipynb
```

Press **CTRL+C** to stop local web server.
