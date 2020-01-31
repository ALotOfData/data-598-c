# data-598-c

## Content
```text
.
├── LICENSE
├── README.md
├── clean_data
│   ├── clean_ramen_ratings.csv
│   └── ramen_features.csv
├── raw_data
│   ├── ramen_consumption_by_country.tsv
│   └── ramen_ratings.csv
└── src
    ├── data_cleaning.ipynb
    └── feature_selection.ipynb
```

| File                                       | Description                                                                                                                            |
| ------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------- |
| LICENSE                                    | Contains license for code in this repository.                                                                                          |
| README.md                                  | This file.                                                                                                                             |
| clean_data/clean_ramen_ratings.csv         | Variables were cleaned and supplemented with additional country based data.                                                            |
| clean_data/ramen_features.csv              | Output of the feature_selection notebook containing extracted features from the ramen_features.csv file.                               |
| raw_data/ramen_consumptions_by_country.tsv | Ramen consumptions by country obtained from the [World instant noodle association](https://instantnoodles.org/en/noodles/market.html). |
| raw_data/ramen_ratings.csv                 | Ramen ratings were obtained from the [kaggle website](https://www.kaggle.com/residentmario/ramen-ratings).                             |
| src/data_cleaning.ipynb                    | Jupyter notebook explaining the initial data cleaning steps.                                                                           |
| src/feature_selection.ipynb                | Jupyter notebook extracting features for classification task.                                                                          |

## Data sources

### Ramen ratings

The original kaggle dataset of ramen ratings posting provides the original source:
> _"This dataset is republished as-is from the original BIG LIST on https://www.theramenrater.com/."_ - Aleksey Bilogur

| Column   | Description                                                            |
| -------- | ---------------------------------------------------------------------- |
| Review # | Review # of the ramen Variety on theramenrater website.                |
| Brand    | Name of instant noodle maker                                           |
| Variety  | Specific name of instant noodle product                                |
| Style    | Format of instant noodle product                                       |
| Country  | Country manifacturer of instant noodle product                         |
| Stars    | Ratings in as a floating point number between 0 and 5                  |
| Top Ten  | Ranking of the instant noodle product is part of the BIG LIST top ten. |

### Ramen consumption by country

The dataset coming from the [World instant noodle association](https://instantnoodles.org/en/noodles/market.html) is an html table extracted from their website on 01/26/2020.

| Column           | Description                                                             |
| ---------------- | ----------------------------------------------------------------------- |
| Country / Region | Country / Region of interest                                            |
| 201*             | Year columns for which consumptions in million of servings was recorded |

## Project description
This project will explore different clustering methods with the goal of predicting instant noodles ratings for the class data 598c at the University of Washington.