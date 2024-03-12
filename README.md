# Sigma wedge Hackathon
## Building a Minimalist trading workflow using Quantrocket
## Description
  This repository involves leveraging the Quantrocket platform to extract Apple stock price data from freely available us-stock price dataset. **The goal is to design a minimalist trading workflow aimed at maximizing portfolio value and identifying optimal buy indices.** The process includes calculating returns percentage, determining market states (Bull, Flat, Bear), and assessing portfolio value. Additionally, a Transition Probability matrix is constructed and normalized to understand market dynamics. Finally, an ARIMA model is implemented to visualize trends in the data, providing insights for informed trading decisions.

## Steps followed 
1. Installation of Docker
2. Installation of Quantrocket
3. Extraction of data
   - Setting up with License key
   - Creating us-stock db
   - Creating universe
   - Getting securities
   - Retrieving the historical data
4. Calculation of returns
5. Identification of the States(Bull or Flat or Bear)
6. Identification of Portfolio values
7. Finding TPM and Normalizing it
8. Maximizing the Portfolio value(V(N))
9. Identifying optimal buy indices
10. Visualizing trends using ARIMA

## Libraries used
1. quantrocket
2. pandas
3. numpy
4. matplotlib
5. seaborn
6. statsmodel
7. sklearn

## Output
  **Maximized value of V(N)** is 17 <br/>
  
  **Optimal buy indices are:** <br/>
    [5, 7, 11, 15, 20, 27, 29, 40, 49, 51, 58, 60, 68, 78, 84, 87, 93, 99, 102, 107, 109, 112, 116, 119, 122, 132, 141, 159, 163, 176, 186, 190, 206, 208, 211, 215, 217, 231, 233, 237]
