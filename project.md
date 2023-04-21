---
# Page settings
layout: default

title: Recommendation Engine
description: Let's build our recommendation engine.  We'll start by cleaning our data. Then we'll prepare our features.  Finally, we'll build our engine!

---

## Step 0

Let's read in our data from our csv and then inspect it.

```
import pandas as pd
from typing import List
from utils.cleaning import lower_case_and_strip_spaces
from utils.cleaning import combine_genres_list
```


```
movies_df: pd.DataFrame = pd.read_csv('input/all_movies.csv')
movies_df.sample(20)
```

```
movies_df
```

```
movies_df.shape[0]
```