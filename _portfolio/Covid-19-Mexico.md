---
title: "Covid-19 in Mexico"
excerpt: "Some statistics extrated from the open dataset from the Mexican Goverment.    <br/><img src='/images/ages.jpg'  >"
collection: portfolio
header-includes: |
    \usepackage{tikz,pgfplots}
---

The dataset is public and is periodically update can be consulted [here](https://datos.gob.mx/busca/dataset/informacion-referente-a-casos-covid-19-en-mexico).
I made this analysis at the begining of the Covid-19 Pandemic in Mexico the data was consulted in April 2020.
<br/>
<br/>
The next graph show us the new cases per day.
<br/><img src='/images/Covid19/nd.png' width="500" height=auto>

We can see the cumulative confirmed cases. 
<br/><img src='/images/Covid19/ct.png' width="500" height=auto>

In the next graph we have the distribution of the age of the patients.
<br/><img src='/images/Covid19/edad.png' width="500" height=auto>


The next graph show us the time between the onset of symptoms and hospitalization.
<br/><img src='/images/Covid19/TH.png' width="500" height=auto>

<br/>

The next graph show us the time between the onset of symptoms and death.
<br/><img src='/images/Covid19/TD.png' width="500" height=auto>

<br/>
We ajust a logist model in oder to predict if a patient is going to required intensive care (ICU) or not based on the comorbidities. 
the logistic ecuation is
<br/>
$$
P(Y=1|X=x)=\frac{1}{1+e^{-\theta^tx}}.
$$
<br/>
Using the maximun likehood principle we can find the vector of coefitients $\theta$. After that we made a hypothesis test in order to find wich variables are significant to predict the probability of requiring ICU.
<br/><img src='/images/Covid19/Captura.PNG'  width="500" height=auto>

