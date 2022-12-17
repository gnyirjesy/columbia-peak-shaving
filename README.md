# columbia-peak-shaving

## Motivation

Our main motivation for this project has been to evaluate possible alternatives to reduce Columbia's University electricity bill. In order to do that, we must first understand the main components of Columbia’s electricity bill, which can be split into two parts. The first part of the bill is given by Columbia’s electricity consumption times a fixed electricity rate of $0.13/kWh, which is determined by its supply-demand contract with the utility company. The second, more significant part, consists of the peak demand charge. To calculate the peak demand charge, the utility identifies the two highest consecutive 15 minute intervals of demand and multiplies it by the respective on-peak/off-peak tariff.

Our goal is to reduce the peak demand charge by leveling out peaks in electricity use. In this case, we will use energy storage to shave off the peaks in consumption. We have the option of using a thermal or a lithium-ion battery, each with its own financial and operational characteristics.

## Results 

Through this study we can conclude that a significant reduction of Columbia’s current electricity bill can be achieved with the 290 kW lithium-ion battery. We achieved an annual cost savings of $85,449.32 in 2019, a NPV for 10 years of $254,371.89 and an IRR of 23.56%. With the battery we can accomplish a peak demand charge reduction of $41,437 (1,659 kW) in 2019. Because of the lithium-ion energy storage's single-trip efficiency of 95%, not all
electricity reaches the battery. Therefore, we need to account for the efficiency losses when charging and discharging the battery. The demand-supply contract's electricity price of $0.13/kWh is considered for this calculation. The annual efficiency lost when charging and discharging the battery equals 36.8 MWh, resulting in an annual cost of $4,791.

## Folder Structure

The repo is structured as follows: 

```
├── README.md
├── archive
├── background
├── battery_operation_2018_daily_optimization.ipynb
├── battery_operation_2019_daily_optimization.ipynb
├── data
│   ├── 2018_results
│   ├── 2019_results
├── peak_shaving_optimization.ipynb
├── stlf_forecast_operation_2019.ipynb
├── ts_forecast.Rmd
├── ts_forecast.html
└── ts_forecast.pdf

```
Important code files are listed on the main repo page. Results can be found in the 2018_results and 2019_results folders.