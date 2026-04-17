# ✈️ Airlines Flight Dataset — Data Analysis

A comprehensive exploratory data analysis (EDA) of India's domestic flight booking data using Python and Pandas.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Features](#features)
- [Analysis Questions](#analysis-questions)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [License](#license)

---

## Overview

This project analyses a flight booking dataset scraped from a popular travel website. The dataset contains records of domestic flight travel between major Indian cities and covers details such as airline, source/destination city, departure/arrival time, number of stops, seat class, duration, days left before departure, and ticket price.

The analysis is intended to be useful for professionals and enthusiasts in the **Airlines** and **Travel** domains.

---

## Dataset

| Property | Details |
|---|---|
| File | `airlines_flights_data.csv` |
| Total Records | ~300,000 rows |
| Format | CSV |

### Airlines Covered

| Airline | Code Prefix |
|---|---|
| AirAsia | I5 |
| Air India | AI |
| GO FIRST | G8 |
| IndiGo | 6E |
| SpiceJet | SG |
| Vistara | UK |

### Cities Covered

Delhi, Mumbai, Bangalore, Chennai, Hyderabad, Kolkata

---

## Features

| Column | Type | Description |
|---|---|---|
| `airline` | Categorical | Name of the airline (6 airlines) |
| `flight` | Categorical | Unique flight code |
| `source_city` | Categorical | Departure city (6 cities) |
| `departure_time` | Categorical | Time-of-day bin for departure (6 labels) |
| `stops` | Categorical | Number of stops: `zero`, `one`, `two_or_more` |
| `arrival_time` | Categorical | Time-of-day bin for arrival (6 labels) |
| `destination_city` | Categorical | Arrival city (6 cities) |
| `class` | Categorical | Seat class: `Economy` or `Business` |
| `duration` | Continuous | Total flight duration in hours |
| `days_left` | Integer | Days between booking date and departure date |
| `price` | Integer | Ticket price in INR (**target variable**) |

---

## Analysis Questions

The Jupyter notebook (`Airlines-Flights-Data-Analysis.ipynb`) answers the following questions:

1. **Q1** — What are the airlines in the dataset, accompanied by their frequencies?
2. **Q2** — Show bar graphs representing Departure Time & Arrival Time distributions.
3. **Q3** — Show bar graphs representing Source City & Destination City distributions.
4. **Q4** — Does price vary with airlines?
5. **Q5** — Does ticket price change based on departure time and arrival time?
6. **Q6** — How does the price change with change in source and destination city?
7. **Q8** — How does the ticket price vary between Economy and Business class?
8. **Q9** — What is the average price of a Vistara flight from Delhi to Hyderabad in Business Class?

---

## Technologies Used

- **Python 3**
- **Pandas** — data loading and manipulation
- **NumPy** — numerical operations
- **Matplotlib** — plotting
- **Seaborn** — statistical visualisations
- **Jupyter Notebook** — interactive analysis environment

---

## Getting Started

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Run the Notebook

```bash
git clone https://github.com/technicalabinesh/Airlines-Flight-Dataset.git
cd Airlines-Flight-Dataset
jupyter notebook Airlines-Flights-Data-Analysis.ipynb
```

> **Note:** Update the `read_csv` path in the notebook's import cell to point to `airlines_flights_data.csv` in the cloned directory.

---

## License

This project is licensed under the terms of the [LICENSE](LICENSE) file included in this repository.