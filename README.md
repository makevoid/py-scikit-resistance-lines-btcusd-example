# Try SciKit ML Charts

### Automatically find resistance lines in pricing trading data 

This repo has an example of an annotated SciKit Learn example of ML Classification using the Clustering Algo Meanshift

The target of this code is to find resistance lines in trading chart data (OHLC)

A possible use case would be to overlay them on DSX

The target was to have a useful example with very little code


### Installation


pip install -r requirements.txt


### Running 

First of all, download some data to play around or unzip and use the dataset in data/sample.csv.zip. This contains data for EURUSD for 2014 and a couple of months for 2015.

Then run the ml.py
> python ml.py data/sample.csv

When the algorithm completes, start a python webserver

> python3 -m http.server 3000

or 

> python -m SimpleHTTPServer 3000

and open your browser to http://0.0.0.0:3000/chart.html


### Docs

https://scikit-learn.org/stable/modules/generated/sklearn.cluster.MeanShift.html

https://aws.amazon.com/blogs/machine-learning/amazon-sagemaker-adds-scikit-learn-support/
