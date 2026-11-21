# 71.7 percent-of-Orders-Fell-Below-Average.-Here-s-Why-That-s-Normal
A boutique owner’s order data goes through health checks, skewness, robust statistics, normality tests, the CLT, bootstrap, and Monte Carlo — with reproducible numbers.
Here are two numbers from the same online-store dashboard: Average Order Value = ₹1,556, and 71.7% of orders below it. Both are correct. The mean is not lying; it is answering a narrower question than the owner is asking.
That gap is not a data error. It is the gap between a dashboard number and an analysis. This article follows one order-amount column through eleven steps — health checks, centre and spread, shape, charts, normality, transformation, the CLT, confidence intervals, bootstrap, a hypothesis test, and a Monte Carlo forecast — so Priya can answer not just “how much?” but “how spread out, how sure, and what next?”
Meet Priya and her dashboard
Priya is a made-up boutique owner. The data is synthetic: 1,002 order records generated in Python with a fixed random seed, and built to look like real online retail, which is messy and right-skewed.
Last Tuesday her dashboard showed one tile: AOV = ₹1,556. The marketing team was pleased.
Priya was not sure. Most customers she knew bought one or two items, a kurta or a scarf, and spent around ₹1,100. So who was spending ₹1,556?
“The average is fine,” her marketing lead said. “Why are you worried?”
“Because I have to order stock and plan next month,” Priya said. “I need to know what a typical customer spends, how much a few big orders are pulling the number up, and whether I can trust this data for forecasting.”
That is the gap between a dashboard number and an analysis. Priya needs a full univariate workflow, meaning she studies one numerical column at a time, and goes deep.
Here is the roadmap:
•	Basic: health check, centre, spread, shape, charts (Steps 1 to 5)
•	Intermediate: normality, transformation, the Central Limit Theorem, confidence intervals (Steps 6 to 8)
•	Advanced: bootstrap, hypothesis test with effect size, Monte Carlo simulation (Steps 9 to 11)
A single dashboard number answers “how much?” An analysis answers “how is it spread, how sure are we, and what happens next?
