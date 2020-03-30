Fourier Series approximation for a hat function. Following youtube series by Steve Brunton https://www.youtube.com/watch?v=dZrShAGqT44&list=PLMrJAkhIeNNT_Xh3Oy0Y4LTj0Oxo8GqsC&index=7. From his book Data Driven Science & Engineering: Machine Learning, Dynamical Systems, and Control by S. L. Brunton and J. N. Kutz Cambridge Textbook, 2019 Copyright 2019, All Rights Reserved

Have matlab version and python version within repository.

Matlab https://github.com/shansiddi/fourierseries/blob/master/fouriers.m

Python https://github.com/shansiddi/fourierseries/blob/master/fouriers.ipynb

General point is that more terms of a Fourier Series taken the better the approximation in general. We find monotomic decrease in error with increasing mode number. Works for nice (continuous) periodic functions like the hat function shown. Why does this work you may ask? Sines and Cosines are a basis for the Hilbert Space. Hilbert Space is the space of all L2 square integrable functions. L2 square integrable functions are functions f which have a bounded integral f^2. So, given an L2 square integrable function f, we can write it in terms of sines and cosines. Generally this Fourier Series has infinite terms, but we can truncate it early and get an approximation that isn't too bad. More terms the better generally. One thing we must watch for however is the Gibbs phenomena. A horrible ringing for our discontinuous functions near the discontinuities. Truncating the Fourier Series will not produce jump discontinuities. Gibbs phenomena is shown with the top hat function.

Also in the repository we have the Gibbs phenomena shown.

Gibbs in Python https://github.com/shansiddi/fourierseries/blob/master/Gibbs.ipynb

Figure 1 shows the hat function by itself. A little sharp, but still continuous, so a nice fourier series can be produced even with just 7 terms. Figure 2 shows the Fourier Series approximations from 1 to 7 terms of the hat function.

<p align="center">
<img src="https://raw.githubusercontent.com/shansiddi/fourierseries/master/images/fig0.PNG">
<p align="center">
<b>Figure 1: Hat function</b><br>
</p>  
 
<p align="center">
<img src="https://raw.githubusercontent.com/shansiddi/fourierseries/master/images/fig1.PNG">
<p align="center">
<b>Figure 2: Hat function with successive Fourier Series approximations superimposed on top</b><br>
</p>   

As previously discussed these truncated Fourier Series give better and better approximations for more terms. Figure 3 represents how the error decreases as modes increase.

<p align="center">
<img src="https://raw.githubusercontent.com/shansiddi/fourierseries/master/images/fig2.PNG">
<p align="center">
<b>Figure 3: Plots of Mode Amplitude and Reconstruction Error vs Mode Number</b><br>
</p> 

With the great computational power however comes great responsibility. In practice we sometimes come across discontinuous functions like the top hat shown in black in figure 4. The red shows the Fourier Series approximation with 100 terms.

<p align="center">
<img src="https://raw.githubusercontent.com/shansiddi/fourierseries/master/images/fig3.PNG">
<p align="center">
<b>Figure 4: Gibbs Phenomena, black is original top hat function, red is Fourier Series approximation</b><br>
</p> 

