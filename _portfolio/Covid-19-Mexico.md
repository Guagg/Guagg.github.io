---
title: "Covid-19 in Mexico"
excerpt: "Some statitis extrated from the open dataset from the Mexican Goverment.    <br/><img src='/images/ages.jpg'  >"
collection: portfolio
header-includes: |
    \usepackage{tikz,pgfplots}
---

The dataset is public and can be consulted [here](https://datos.gob.mx/busca/dataset/informacion-referente-a-casos-covid-19-en-mexico).

<br/><img src='/images/Covid19/nd.png' width="500" height=auto>
<br/><img src='/images/Covid19/ct.png' width="500" height=auto>
<br/><img src='/images/Covid19/edad.png' width="500" height=auto>
<br/><img src='/images/Covid19/TD.png' width="500" height=auto>
<br/><img src='/images/Covid19/TH.png' width="500" height=auto>

We ajust a logist model in oder to predict if a patient is going to required intensive care (ICU) or not based on the comorbidities. 
the logistic ecuation is
$$
P(Y=1|X=x)=\frac{1}{1+e^{-\theta^tx}}
$$
and using the maximun likehood principle we can find the vector of coefitients $\theta$. After that we made a hypothesis test in order to find wich variables are significant to predict the probability of requiring ICU.


<br/><img src='/images/Covid19/Captura.PNG'  width="500" height=auto>

