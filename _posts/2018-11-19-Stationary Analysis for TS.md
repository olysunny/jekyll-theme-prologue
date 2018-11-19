---
title: Stationary Analysis for Time Series Model
layout: post
---
<h2>The Concepts and examples of Unit-root tests and stationarity tests</h2>
<div class="row">
		<div class="6u 12u$(small)">
    
    <h3>Concept of Unit-root tests:</h3>
    <ul>
         <li>Null hypothesis: Unit-root</li>
         <li>Alternative hypothesis: Process has root outside the unit circle, which is usually equivalent to stationarity or trend stationarity</li>
    </ul>
    
    <h3>Concept of Stationarity tests</h3>
    <ul>
        <li>Null hypothesis: (Trend) Stationarity</li>
        <li>Alternative hypothesis: There is a unit root.</li>
    </ul>
    </div>
 </div>
 
<h2>There are many different Unit-root tests and many Stationarity tests.</h2>
<div class="row">
  <div class="6u 12u$(small)">
    <h3>Some Unit root tests:</h3>
    <ul>
         <li>Dickey-Fuller test</li>
         <li>Augmented Dickey Fuller test</li>
         <li>Phillipps-Perron test</li>
         <li>Zivot-Andrews test</li>
         <li>ADF-GLS test</li>
    </ul>
    The most simple test is the DF-test. The ADF and the PP test are similar to the Dickey-Fuller test, but they correct for lags. The ADF does so by including them the PP test does so by adjusting the test statistics.

    <h3>Some Stationarity tests:</h3>
    <ul>
        <li>KPSS</li>
        <li>Leybourne-McCabe</li>
    </ul>
    <p>In practice KPSS test is used far more often. The main difference of both tests is that KPSS is a non-parametric test 
    and Leybourne-McCabe is a parametric test.</p>
  </div>
</div>  











How unit-root test and stationarity-test complement each other
If you have a time series data set how it usually appears in econometric time series I propose you should apply both a Unit root test: (Augmented) Dickey Fuller or Phillips-Perron depending on the structure of the underlying data and a KPSS test.

Case 1 Unit root test: you can’t reject H0; KPSS test: reject H0. Both imply that series has unit root.

Case 2 Unit root test: Reject H0. KPSS test: don't reject H0. Both imply that series is stationary.

Case 3 If we can’t reject both test: data give not enough observations.

Case 4 Reject unit root, reject stationarity: both hypotheses are component hypotheses – heteroskedasticity in a series may make a big difference; if there is structural break it will affect inference.

Power problem: if there is small random walk component (small variance σ2μ), we can’t reject unit root and can’t reject stationarity.

Economics: if the series is highly persistent we can’t reject H0 (unit root) – highly persistent may be even without unit root, but it also means we shouldn’t treat/take data in levels. Whether a time series is "highly persistent" can be measured with the p-value of a unit-root test. For a more detailed discussion what "persistence" means in time-series see: Persistence in time series

General rule about statistical testing You cannot proove a null hypothesis, you can only affirm it. However, if you reject a null hypothesis then you can be very sure that the null hypothesis is really not true. Thus alternative hypothesis is always a stronger hypothesis than the null hypothesis.

Variance ratio tests:

If we want to quantify how important the unit root is, we should use a variance ratio test.

In contrast to unit root and stationarity tests, variance ratio tests can also detect the strength of the unit root. The outcomes of a variance ratio test can be divided into roughly 5 different groups.

Bigger than 1 After the shock the value of the variable explodes even more in the direction of the shock.

(Close to) 1 You get this value in the "classical case of a unit root"

Between 0 and 1 After the shock the value approaches a level between the value before the shock and the value after the shock.

(Close to) 0 The series is (close to) stationary

Negative After the shock the value goes into the opposite direction, i.e. if the value before the shock is 20 and the value after the shock is 10 over the long haul the variable will take on values greater than 20.
