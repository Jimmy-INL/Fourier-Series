Fourier Series approximation for a hat function. Following youtube series by Steve Brunton https://www.youtube.com/watch?v=dZrShAGqT44&list=PLMrJAkhIeNNT_Xh3Oy0Y4LTj0Oxo8GqsC&index=7. From his book Data Driven Science & Engineering: Machine Learning, Dynamical Systems, and Control by S. L. Brunton and J. N. Kutz Cambridge Textbook, 2019 Copyright 2019, All Rights Reserved

Have matlab version and python version within repository.

Matlab https://github.com/shansiddi/fourierseries/blob/master/fouriers.m

Python https://github.com/shansiddi/fourierseries/blob/master/fouriers.ipynb

General point is that more terms of a Fourier Series taken the better the approximation in general. We find monotomic decrease in error with increasing mode number. Works for nice (continuous) periodic functions like the hat function shown.

<p align="center">
<img src="https://raw.githubusercontent.com/shansiddi/fourierseries/master/images/fig0.PNG">
<p align="center">
<b>Hat function</b><br>
</p>  
 
<p align="center">
<img src="https://raw.githubusercontent.com/shansiddi/fourierseries/master/images/fig1.PNG">
<p align="center">
<b>Hat function with successive Fourier Series approximations superimposed on top</b><br>
</p>   

<p align="center">
<img src="https://raw.githubusercontent.com/shansiddi/fourierseries/master/images/fig2.PNG">
<p align="center">
<b>Plots of Mode Amplitude and Reconstruction Error vs Mode Number</b><br>
</p> 
