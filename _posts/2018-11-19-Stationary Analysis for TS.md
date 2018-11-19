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
    <p>The most simple test is the DF-test. The ADF and the PP test are similar to the Dickey-Fuller test, but they correct for lags. The ADF does so by including them the PP test does so by adjusting the test statistics.</p>

    <h3>Some Stationarity tests:</h3>
    <ul>
        <li>KPSS</li>
        <li>Leybourne-McCabe</li>
    </ul>
    <p>In practice KPSS test is used far more often. The main difference of both tests is that KPSS is a non-parametric test 
    and Leybourne-McCabe is a parametric test.</p>
  </div>
</div>  


<h2>How unit-root test and stationarity-test complement each other</h2>
<p>If you have a time series data set how it usually appears in econometric time series I propose you should apply both a Unit root test: <b>(Augmented) Dickey Fuller or Phillips-Perron</b> depending on the structure of the underlying data and a <b>KPSS</b> test.</p>

<div class="row">
   <div class="6u 12u$(small)">
	   <ul>
		   <li>Case 1 Unit root test: you can’t reject H0; KPSS test: reject H0. Both imply that series has unit root.</li>
		   <li>Case 2 Unit root test: Reject H0. KPSS test: don't reject H0. Both imply that series is stationary.</li>
		   <li>Case 3 If we can’t reject both test: data give not enough observations.</li>
		   <li>Case 4 Reject unit root, reject stationarity: both hypotheses are component hypotheses – heteroskedasticity in a series may make a big difference; if there is structural break it will affect inference.</li>
            </ul>
	   <ul>
		   <li>Power problem: if there is small <em>random walk component</em> (small variance σ2μ), we can’t reject unit root and can’t reject stationarity.</li>
		   <li>Economics: if the series is highly persistent we can’t reject H0 (unit root) – highly persistent may be even without unit root, but it also means we shouldn’t treat/take data in levels. Whether a time series is "highly persistent" can be measured with the p-value of a unit-root test. For a more detailed discussion what "persistence" means in time-series see: <a href="https://stats.stackexchange.com/questions/11927/persistence-in-time-series">Persistence in time series</a></li>
	   </ul>
     </div>
  </div>
		   
<h2>Variance ratio tests:</h2>
<p>If we want to quantify how important the unit root is, we should use a variance ratio test.</p>
<p>In contrast to unit root and stationarity tests, variance ratio tests can also detect the strength of the unit root. The outcomes of a variance ratio test can be divided into roughly 5 different groups.</p>
<div class="row">
   <div class="6u 12u$(small)">
	   <ul>
		   <li>Bigger than 1: After the shock the value of the variable explodes even more in the direction of the shock.</li>
	           <li>(Close to) 1: You get this value in the "classical case of a unit root".</li>
		   <li>Between 0 and 1: After the shock the value approaches a level between the value before the shock and the value after the shock.</li>
		   <li>(Close to) 0: The series is (close to) stationary</li>
		   <li>Negative: After the shock the value goes into the opposite direction, i.e. if the value before the shock is 20 and the value after the shock is 10 over the long haul the variable will take on values greater than 20.</li>
            </ul>
    </div>
</div>
