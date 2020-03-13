# Coronavirus. Simulation of Poland.

This program is a mathematically possible interpretation of the course of coronavirus infections in Poland.
The considerations are based on mathematical insights on the development of the disease in Central and Western Europe, they are quite general, but correctly depict the scenario of the future.
I use Python to create most charts and I use C++ to create a simple simulation.

## General considerations.

A resident of Zielona Góra became the first patient in Poland diagnosed with coronavirus. It happened on March 4, 2020.
At the time of this "text" (March 13), we have 51 cases of this virus infection in Poland. What's next?

Consider the coronavirus chart:

![picture1](./images/corona1.png)

The epidemic image is a pattern of an exponential function in the field of natural numbers (days), for each day the value of the function takes values greater by the product of a fixed number compared to the previous day. What is this "constant number"? It turns out to be a value between 1.11 and 1.27.

However, let's look at the logarithmic function of coronavirus:

![picture2](./images/corona2.png)

The exponential increase looks like a straight line, we find that the value of the function increases on average ten times every 16 days. This is terrifying, it would mean that after 64 days in the world the number of infected will be 100 million people!  However, we can be calm: this line does not go on forever, eventually the function will stop growing exponentially. Why? The first option: the whole world will be infected, so you can no longer infect anyone. The second option is based on considering the past. For example: "Spanish flu" (1918) stopped after 513 million infections. However, we do not know if (and when) this will happen in the case of a coronavirus...

## Methodology.

In general, two cases of virus spread should be considered. First: people are completely isolated from each other. Second: people move freely. Of course, we accept the second "case", because you can not thoughtlessly assume that everyone will spend all time in quarantine.

![picture3](./images/corona3.png)
