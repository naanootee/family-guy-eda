**Family Guy — Exploratory Data Analysis**
Family Guy data analysis project using Python. Analysis of 400 episodes across 21 seasons, exploring IMDb rating trends, musical episodes, guest stars, writers/directors, runtime impact, and character appearances through EDA and data visualization on Family Guy.

* What does 21 seasons of data actually tell us about one of the longest-running animated shows in history? *
This project explores **400 episodes of Family Guy** through IMDb ratings, musical numbers, guest stars, and special episodes — with a visual style inspired by the show itself.

---

## What's inside

| Section | What it covers |
|---|---|
| Ratings Overview | How ratings evolve across 21 seasons, best/worst episodes per season, full episode heatmap |
| Directors & Writers | The most prolific names behind the camera and at the keyboard |
| Musical Episodes | Do episodes with songs rate higher? Which songs keep coming back? |
| Guest Stars | Rating impact of guest stars, who appears most, and volume vs quality |
| Special Episodes | Do longer episodes earn their runtime? All 7 specials ranked |

---

## Key findings

- **Seasons 4–5 were the peak** — ratings have been on a slow but clear downward trend since then, with increasing inconsistency in later seasons.
- **Musical episodes score +0.24 points higher** on average. The effect is consistent across most seasons and rises to +0.4 in seasons 3, 6, and 13.
- **Guest stars help, but less than you'd think** — a +0.17 average boost that almost disappears in later seasons. Wallace Shawn (3 eps, avg 7.93) outperforms Carrie Fisher (9 eps, avg 7.28).
- **Every single special (44+ min) scores above the series mean** — specials average 7.94 vs 6.96 for standard episodes.

---

## Tools & libraries

Python
Pandas
Matplotlib
Seaborn

---

## Repository structure

```
family-guy-eda/
├── FamilyGuy_Final.ipynb          ← main analysis notebook
├── character_appearances.ipynb    ← bonus: fixing a data parsing bug on character counts
├── data/
│   └── Family Guy Dataset.csv     ← source dataset (from Kaggle, see link below)
├── fonts/
│   ├── LuckiestGuy-Regular.ttf    ← free via Google Fonts
│   └── ComicNeue-Regular.ttf      ← free via Google Fonts
└── README.md
```

---

## How to run it

**1. Clone the repo**
```bash
git clone https://github.com/naanootee/family-guy-eda.git
cd family-guy-eda
```

**2. Install dependencies**
```bash
pip install pandas numpy matplotlib seaborn
```

**3. Download the fonts** (optional but recommended for the cartoon style)
- [Luckiest Guy](https://fonts.google.com/specimen/Luckiest+Guy) → save as `fonts/LuckiestGuy-Regular.ttf`
- [Comic Neue](https://fonts.google.com/specimen/Comic+Neue) → save as `fonts/ComicNeue-Regular.ttf`

If the fonts aren't found, the notebook falls back to the system default — the analysis still runs fine.

**4. Download the dataset**

The dataset is not included in the repo due to file size. Download it from Kaggle and place it at `data/Family Guy Dataset.csv`:

[Family Guy Dataset — Kaggle](https://[www.kaggle.com/datasets/iamsouravbanerjee/family-guy-dataset])

**5. Open the notebook**
```bash
jupyter notebook FamilyGuy_eda.ipynb
```

## Dataset

**Family Guy Dataset** from Kaggle — 400 episodes, 21 columns including IMDb ratings, U.S. viewership, running time, directors, writers, guest stars, and musical numbers.

---

*Made by [Nano Vives][https://www.linkedin.com/in/nano-vives/] · 2026*
