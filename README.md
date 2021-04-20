# Stock Market Regime Detection using Hidden Markov Models

## What is a Markov Model?

The classic textbook example of a Markov model is the weather. We classify days as, say, sunny, cloudy, or raining. Then, we pick a transition period (let's assume 1 day) and determine estimates of the transition probabilities. There will be nine of these (because there are three states). So, for example, we need the probably that tomorrow will be sunny given that today is sunny, the probably that tomorrow will be cloudy given that today is sunny, and so on.

How do we estimate values of the transition probabilities in this model? We go outside and observe the weather for, say, 100 days. Each transition probability is just the number of transitions of that type we observed divided by 100. 

![alt text](https://github.com/andrewritchie05/Stock_Market_Regime_Detection/blob/main/Picture1.png?raw=true)

## What is a Hidden Markov Model?

Suppose now that we work/live in a windowless building. We can't directly observe the weather, so we can't establish the transition probabilities in our model anymore. However, suppose we can observe some phenomenon related to the weather, like how many people bring umbrellas to the office. Or how may people are wearing shorts or sunglasses. This tells us something about the weather, but only in terms of probability. If there's lots of umbrellas, say, it likely today it is raining but we can't say that with 100% certainty, so we must use probability.

We could make an (ordinary) Markov model based on umbrellas, shorts, and sunglasses. However, we are still interested in the original model of sunny, cloudy, and raining. That model is hidden from us. Hence, Hidden Markov Model.

## Applying this to Financial Markets

- Tweaking the above example of weather, we can apply it to financial markets. 
- Instead of Sunny/Cloudy/Rainy we will assume 3 different market states: Bull, Bear, Neutral
-	Instead of Sunglasses/Shorts/Umbrellas, variables of interest will be those related to financial markets: OHLC/Volume/Measures of change in these etc.


