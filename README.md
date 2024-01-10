# Options Pricing using Deep Learning
## Breakdown
We use the Functional API within Keras to create a multi-model framework, in which multiple individual neural networks feed forward into one singular final funnel. This separation serves to provide clarity between variables; each individual funnel represents one factor within options pricing. More specifically, the three funnels represent the Greeks, the market state, and information about the derivative itself. There is overlap within each funnel, as some variables prove useful in multiple factors (like strike price). 

Using neural networks to price an option contract allows us to evade common (and often flawed) assumptions, such as constant volatility. As we are solely approximating a multivariate function to a contract price, the only required assumption is that our sample data is representative of the population data. 
