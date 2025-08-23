# Reddit_sentiment
Codes for the paper: Modeling Sentiment Spread in Reddit’s Financial Communities through Epidemiological and Deep Learning Approaches

To assign positive or negative sentiment to Reddit sumbissions and comments we used the codes in 1_step.ipynb, 2_step.ipynb, 3_step.ipynb.

In 1_step.ipynb we upload and filter data, then we perform the first classification using the zero-shot approach.
In 2_step.ipynb we do the training using labels obtained by the zero-shot approach.
In 3_step.ipynb we do the final classification using the model trained in 2_step.ipynb.

In Network_creation.ipynb we create the network for each company, considering links between users replying to a submission and authors of the submission, and between users replying to a comment and authors of the comment.

In Experiments_code.ipynb there is the code with the definition of the ABM and both its calibration and validation. Moreover there are comparisons with an ODE SIS and a SIS on network without trust. 

Data:
  - apple_sentiment_series.json, amazon_sentiment_series.json, google_sentiment_series.json are the file containing the percentage of positive and negative posts for each week.
  - apple_network_5_months_right_sentiment.graphml, amazon_network_5_months_right_sentiment.graphml, google_network_5_months_right_sentiment.graphml are the files containing the networks with nodes initialized with positive or negative sentiment.
