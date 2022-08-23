# QuantumVal


Quantum approximate optimisation algorithms for real-world scenarios --> by Strangeworks

 Name of the team : QuantumVal
 
 
 Name of all the members : Grishma Prasad,Abha Naik & Shivani  Rajput


Grishma Prasad :
                     Discord Id: Grishma#4171
                     Github Id: https://github.com/gprs1809
                     Email Id: 


Abha Naik :
          Discord Id: ABHANAIKIM(IST)#5826
                    Github Id: https://github.com/AbhaSNK
                    Email Id: abhanaikimq@gmail.com


Shivani Rajput :
          Discord Id: Shivani Rajput#6848
                    Github Id: https://github.com/ShivaniRajput11
                    Email Id: shivanirajput1880@gmail.com






## Introduction:

Problem : We explore QAOA with CVAR approach for portfolio optimization application using different number of assets, backends and classical optimizers and analyze the results.


You can learn more about QAOA here: https://qiskit.org/textbook/ch-applications/qaoa.html

#### Data Extraction: 

We used Yahoo! Finance to get the historical data over 3 months of 10 Indian Stocks: 


MARUTI.NS , ONGC.NS, TATASTEEL.NS, HINDALCO.NS, ICICIBANK.NS, BRITANNIA.NS, ULTRACEMCO.NS, WIPRO.NS, APOLLOHOSP.NS, JUBLFOOD.NS


We used variance method to calculate individual stock risk and covariance to calculate the inter-related risk of all the stocks.
You can have an indepth look at the data in the attached excel sheet (FINANCEDATA 3 MON.xlsx)

#### Backends:


We have initially solved the problem classically using NumPyMinimumEigenSolver(). Linear equality to penalty converter is used on the quadratic problem so that the constraints are taken into account in the objective, making the problem simpler. Converting to an ising model post that.We are using cobyla optimizer and qasm simulator in this case and CVaR expectation and hence, creating a list of alpha values.
