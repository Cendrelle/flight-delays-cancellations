# Flight Delays and Cancellations Analysis

## Project Overview

This project explores flight departure delays and cancellations using flight and weather data from two major airports in the Pacific Northwest: Seattle-Tacoma International Airport (SEA) and Portland International Airport (PDX).

The analysis focuses on the first half of 2022 and aims to identify patterns in flight delays and cancellations across routes, airlines, and weather conditions.

This project was completed as part of a DataCamp data analysis project.

## Business Questions

- Which flight routes experience the highest average departure delays?
- Which routes have the highest number of cancellations?
- Which airlines experience the highest average departure delays?
- Which airlines record the most flight cancellations?
- How are wind gust conditions associated with average departure delays?

## Dataset

The analysis uses two CSV datasets:

- `flights2022.csv`: Flight information, including departure times, delays, airlines, origins, and destinations.
- `flights_weather2022.csv`: Flight information enriched with weather measurements.

The datasets cover flights departing from SEA and PDX during the first half of 2022.

Source: [ModernDive – pnwflights2022](https://moderndive.com/)

## Tools and Libraries

- Python
- Pandas
- Matplotlib

## Methodology

1. Load and inspect the flight and weather datasets.
2. Create flight routes using origin and destination airports.
3. Aggregate departure delays and cancellations by route.
4. Identify routes with the highest average departure delays and cancellation counts.
5. Compare airline performance using average departure delays and cancellation counts.
6. Group flights according to wind gust intensity and compare average departure delays across the two airports.

## Preliminary Findings

The initial analysis suggests that:

- Average departure delays differ across flight routes and airlines.
- Cancellation counts vary across routes and carriers.
- Flights in the higher wind-gust group (at least 10 mph) show higher average departure delays at both airports.

| Airport | Wind gust below 10 mph | Wind gust at least 10 mph |
|---|---:|---:|
| PDX | 6.69 min | 9.15 min |
| SEA | 7.86 min | 9.23 min |

These results describe associations in the observed data and do not establish a causal relationship between wind gusts and flight delays.

## Project Structure

```text
flight-delays-cancellations/
├── README.md
├── notebook.ipynb
├── data/
├── requirements.txt
└── .gitignore
```

## How to Run

1. Clone this repository.
2. Install the required dependencies:

```bash
pip install -r requirements.txt
```

3. Place the two CSV datasets in the `data/` directory.
4. Open the notebook and execute the cells.

## Limitations

- The analysis is limited to two airports and the first half of 2022.
- Weather conditions are examined through selected variables rather than a comprehensive weather model.
- Average delays alone do not capture the full distribution of delays.
- The observed associations should not be interpreted as causal relationships.

## Acknowledgements

This project was completed as part of a DataCamp guided project.

