# Predicting flight departure delays

Course project for **IT4142E – Introduction to Data Science** (HUST).

We predict whether a flight from New York (EWR, JFK, LGA) will leave **at least 15 minutes late**, using only information available before departure (schedule, airline, route). Data: [nycflights13](https://nycflights13.tidyverse.org) (336,776 flights from 2013, CC0).

## Contents

| Path | What it is |
|---|---|
| [`flight_delays_initial_results.ipynb`](flight_delays_initial_results.ipynb) | Initial results: data integration, quality checks, EDA, baselines vs. decision tree vs. Random Forest, evaluation and interpretation |
| [`docs/`](docs/) | Project description and data preparation report |
| `data/` | Downloaded automatically by the notebook (not tracked in git) |

## Running

```bash
pip install -r requirements.txt
jupyter notebook flight_delays_initial_results.ipynb
```

The second cell of the notebook downloads `flights.csv`, `airlines.csv` and `airports.csv` into `data/` if they are missing. Running the notebook end-to-end takes about one minute.
