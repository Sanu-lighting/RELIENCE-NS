# RELIENCE-NS (The Relience NS data is used here)
A model that finds whether the price closing price after 5 days will go up or down. And using this data it predicts how much profit would i make after investing for a certain number of years 
Here in the code I used a trading startagy : 
●	Initial Capital: ₹1,000,000. 
●	Execution:  
○ If your model outputs a 1 on Day T, you Go Long (buy the stock) at the Open price on Day T+1. 
○ If your model outputs a 0 on Day T, you Go Short (short-sell the stock) at the Open price on Day T+1. 
●	The Holding Rule: You must hold the position for exactly 5 trading days, ignoring all new signals generated during this time. 
●	The Exit: You will close your position at the Close price on Day T+5. After closing, wait for the very next signal to re-enter the market. 
 
Return Calculations (100% Capital Allocation per Trade): 
●	Long Return: (𝑂𝑝𝑒𝑛_(𝑇 + 1)/ 𝐶𝑙𝑜𝑠𝑒_(𝑇 + 5) )-1
●	Short𝑇𝑟𝑎𝑑𝑒 Return: 𝑅𝑒𝑡𝑢𝑟𝑛  = (𝐶𝑙𝑜𝑠𝑒_(𝑇 + 5) / 𝑂𝑝𝑒𝑛_(𝑇 + 1)) − 1  
 
●	𝑇𝑟𝑎𝑑𝑒𝑁𝑒𝑤 𝐶𝑎𝑝𝑖𝑡𝑎𝑙 𝑅𝑒𝑡𝑢𝑟𝑛  == capital*(1+return)
I caluculated the return with respect to the past 3 year data (01-01-2021 to 01-01-2024)
