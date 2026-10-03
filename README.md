# DATA 230 Group Project: What makes a London Airbnb listing top rated?

**Question:** which listing and host features predict a top rating (4.8 or higher), so hosts know what to improve first.

## Data
- Source: Inside Airbnb, London, snapshot 19 June 2026, detailed listings file `listings.csv.gz` (92,638 listings × 90 columns), CC BY 4.0.
- The data is not stored in this repo because of its size. Download it from https://insideairbnb.com/get-the-data (London section, "Detailed Listings data", not the summary `listings.csv`).

## How to run
1. Clone this repo with GitHub Desktop (File > Clone Repository).
2. Inside the cloned folder, create a folder named `data` and put `listings.csv.gz` in it. Do not unzip it.
3. Open `notebooks/01_cleaning.ipynb` in Jupyter and run Kernel > Restart Kernel and Run All Cells. This creates `data/listings_clean.csv`.
4. In your own notebook, load the cleaned data with `pd.read_csv("../data/listings_clean.csv")`.

## Folder structure
```
data/        raw and cleaned data (not tracked by Git)
notebooks/   one notebook per task
figures/     saved figures (PNG)
```

## Notebooks and owners
| Notebook | Owner | Purpose |
|---|---|---|
| `00_dataset_check_varuna.ipynb` | Varuna | Dataset comparison and selection |
| `01_cleaning.ipynb` | Varuna | Data quality, cleaning decisions, target `top_rated` |
| `02_univariate` (planned) | Priya | Multivariate and Presentation slides |
| `03_relationships` (planned) | Sanjana | Features vs rating, ML direction |
| `04_cpu_vs_gpu` (planned) | Ngoc | CPU vs GPU (RAPIDS) timing; Tableau dashboard |

## Working rules
- Fetch/Pull before you start; commit and push at least once a day.
- Work only in your own notebook.
- Every figure gets a one-line insight underneath.
