# Solutions-about-risk-management-problems1

1 Retrieve four years of daily data on 1–, 2–, 3–, 5–, 7–, 10–, 20–, and 30–year (nominal) constant maturity yields 
(in percent per annum 3 ) through January 18, 2019, and convert these into log-return timeseries. 

To do this conversion, use the approximation from the Appendix:
log((Pt+∆t)/Pt) ≈ y* ∆t −(1 −(1 +y/2)^(−2τ)/y * ∆y
where y is annual yield rate, t is measured in years, and τ is the bond term (in years).

2  Retrieve four years of daily Treasury financing rates from the NY Fed website and use them to demean the Treasury log-returns

3 Use quasi maximum likelihood to fit GARCH(1,1) to the log-returns and use the conditional variances to standardize the residuals. 
We saw last semester that fixed income assets experience materially leptokurtotic (fat-tailed) innovations. Here we are interested in 
(co)variance, so we need an estimator that is robust to leptokurtosis, such as Maronna’s M-estimator implemented in algorithm 6.29 

4 Use the M-estimator with ν = 3 to estimate the term structure dispersion of the log-returns of Treasury bond prices

Principal component analysis is based on eigenvalues and eigenvectors
5 Calculate the eigenvalues of the dispersion matrix. The established concept of “bond duration” is predicated on an assumption of 
the prominence of systematic risk in (long-only) bond portfolios.How prominent is the largest eigenvector of the dispersion here? If 
you were to build a factor model for the Treasury market, how many factors would you use?
