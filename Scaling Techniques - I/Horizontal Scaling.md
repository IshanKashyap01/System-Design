# Horizontal Scaling

- A more complex option for scaling is to *add more computers* to the system

- Hence, we can use *commodity h/w* and connect them via a *network*

- This form of scaling is known as **horizontal scaling**

- The same components are *replicated* on all the systems *increasing availability*

## Horizontal Scaling a Monolithic Application

1. Maintaing the *consistency* is a big challenge as the entire app needs to be
replicated every time

2. There is *no selective scaling*, i.e. if a component need not be scaled, it'll
still be replicated on all machines
