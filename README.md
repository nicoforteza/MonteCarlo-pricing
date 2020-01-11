# Montecarlo Pricing for Exotic Options
The aim of the following exercise is to price a **call option** in which the underlying asset follows a Constant Elasticity Variance Process (CEV). A CEV process can be written as follows:
\
                <center>**$dSt = \mu Sdt + \sigma S^\gamma dz$**</center>
\
where $dz$ is a _wiener_ process, $\sigma$ is the volatility parameter and $\gamma$ is a positive constant.
Montecarlo simulations are made to simulate the expected and theoretical value of the option. Some conditions that I propose must be cumplimented: 

- There are 3 stages of time for the price of the underlying within the life of the option that must be within an interval, defined by alpha (lower bound) and beta (upper bound). 
- If this condition is **fulfilled**, the payoff activates for that stage of time, otherwise not. The total payoff will be the expected mean of the payoffs of each stage of time.
