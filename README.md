# Google Playstore analysis
An analysis of Google Play Store Apps dataset using CRISP-DM process

# Libraries used

The following libraries are used in the notebook:

```
import pandas as pd
import numpy as np

import matplotlib.pyplot as plt
import seaborn as sns
import plotly.graph_objects as go

from datetime import datetime as dt
import time
import datetime
import re
import functools
import bs4 as BeautifulSoup

from sklearn.model_selection import train_test_split
from sklearn.neighbors import KNeighborsRegressor
```

# Project motivation

My main questions of interest are the following:

- What do high-rated apps have in common?
- What kind of apps are the most popular and well-liked by users?
- What characteristics distinguish paid and free apps from each other?
- Can we predict the rating given the app features this dataset provides?

# Project files

The repo includes the following files:

- 49864_274957_bundle_archive folder that includes data files, namely googleplaystore.csv and googleplaystore_user_reviews.csv
- README.md
- google_play_store.ipynb - the notebook used for analysis

# Summary of findings

- Regular app updates along with size seem like prominent contributors to app ratings
- Ratings have been rounded up. Even though most of our apps are last updated in 2018, the relative distribution of the ratings per year shows a steady increase in - apps rated 4.5 and above from 2015 onwards
- Up-to-date and relatively large app size are two indicators that important indicators that are relatively correlated with high-rated apps
- If we consider another category's app rating ratio - like category - we can see a clear preference for events, parenting, books and reference and art and design.
- Most popular apps are labeled as family, game and tools (38%)
- Nearly a third of all paid apps are rated 4.5 or above compared to a quarter of free apps which achieve such high acclaim

# Acknowledgements

As part of Udacity's Data Science nanodegree, students are required to write a blog post that takes the reader through data analysis of a chosen dataset. If you enjoyed this post please give it a couple of claps.

Medium post for this analysis can be found See [here](https://medium.com/@plan__b/the-state-of-google-play-store-a-data-approach-9402cda5f038?postPublishedType=initial).
