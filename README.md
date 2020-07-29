# Pwc-Competition-July2020
Pwc Competition held in July 2020. Repository contains data(xls) and jupter notebook code.

Objective: Forecast the Operation for Aviation Industry for the next 12 months
Data Source: China Air Transport Association
Data Description: 4 Transportation Metrics of China Aviation Industry from Jan 2018 to June 2020 (aggregated Monthly)
1. Total Traffic Turnover (Billion Ton-Kilometers): Product of transportation volume and average haul distance
2. Passenger Volume(Ten Thousand People) : Number of passengers transported
3. Passenger Turnover (Billion Person-Kilometers): Product of passenger volume and passenger distance
4. Passenger Throughput (Ten Thousand People): Number of passengers entering and leaving the area

Model Selection: Time Series Prediction (SARIMAX)
Assumptions : 
1. The autoregressive model relies on the nearest 4-5 historical values and prediction error values (March to June 2020) 🡪 p,q ∈ (4,5)
2. Due to the data instability caused by COVID-19 , there will not be train/test split. The model is trained on the all data, while the optimal model is obtained by evaluating AIC through parameters iterating. 
3. Prediction will be generated on the next 12 months. 

