# Sigma wedge Hackathon
The python code for AAPL stock price is present in Modified_AAPL.ipynb kindly refer to it
## Building a Minimalist trading workflow using Quantrocket
## Description
  This repository involves leveraging the Quantrocket platform to extract Apple stock price data from freely available us-stock price dataset. **The goal is to design a minimalist trading workflow aimed at maximizing portfolio value and identifying optimal buy indices.** Firstly, the returns corresponding to closing prices are calculated. States are classified, and for each day, transition probabilities are determined. Based on these probabilities, a decision is made whether to buy the stock or not on that specific day. Two states are considered: additive state and reductive state. If the additive state's value is higher than the reductive state's value, the stock is purchased; otherwise, it's not. When buying the stock, the portfolio value is increased by 1. This process is repeated for each day in a **streaming manner** using a value iteration approach to find the optimal buy indices and portfolio value.

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
6. Finding TPM 
7. Based on the TPM calculated for each day decision is made whether to buy or not to buy
8. If stock is bought portfolio value is increamented by 1
9. Finding optimal buy indices
10. Identifying Maximized portfolio value.
   

## Libraries used
1. quantrocket
2. pandas
3. numpy
4. matplotlib
5. seaborn
6. statsmodel
7. sklearn

## Output
  **Maximized value of V(N)** is 16 <br/>
  
  **Optimal buy indices are:** <br/>
    [4, 5, 7, 9, 10, 11, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 29, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 43, 44, 45, 46, 49, 51, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62, 63, 64, 65, 66, 67, 68, 69, 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 88, 89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99, 100, 101, 102, 103, 104, 105, 106, 107, 108, 109, 110, 111, 112, 113, 114, 115, 116, 117, 118, 119, 120, 121, 122, 123, 124, 125, 126, 127, 128, 129, 130, 131, 132, 133, 134, 135, 136, 137, 138, 139, 140, 141, 142, 143, 144, 145, 146, 147, 148, 149, 150, 151, 152, 153, 154, 155, 156, 157, 158, 159, 160, 161, 162, 163, 164, 165, 166, 167, 168, 169, 170, 171, 172, 173, 175, 176, 177, 178, 180, 181, 182, 184, 185, 186, 187, 188, 189, 190, 191, 192, 193, 194, 195, 197, 198, 199, 200, 202, 203, 206, 207, 208, 209, 210, 211, 212, 213, 214, 215, 216, 217, 218, 219, 220, 221, 222, 223, 224, 225, 226, 227, 228, 229, 230, 231, 232, 233, 234, 235, 237, 238, 239, 240, 241, 242, 244, 245, 246, 247, 248, 249]
