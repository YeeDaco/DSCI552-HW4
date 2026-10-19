# DSCI 552 — Homework 4

Binary and multiclass time series classification on the UCI AReM (Activity Recognition system based on Multisensor data fusion) dataset — logistic regression with recursive feature elimination, L1-penalized logistic regression, L1-penalized multinomial regression and Naïve Bayes — plus ISLR exercises 4.8.3 and 4.8.7.

## Structure

```
.
├── README.md
├── .gitignore
├── data
│   └── AReM
│       ├── bending1/ bending2/ cycling/ lying/ sitting/ standing/ walking/   (dataset*.csv)
│       ├── bendingType.pdf
│       └── sensorsPlacement.pdf
├── notebook
│   └── Lu_Yiming_HW4.ipynb
└── requirements.txt
```

## Run

```bash
pip install -r requirements.txt
cd notebook
jupyter notebook Lu_Yiming_HW4.ipynb   # then Kernel -> Restart & Run All
```

The notebook loads data with the relative path `../data/AReM/`. The loading and feature-extraction code from Homework 3 is repeated at the top of the notebook, since Problem 2 needs it. A full run takes a few minutes (the cross-validation over l = 1, …, 20 is the slow part).
