# WEEK-7-BASIC-DATA-ANALYSIS
# TASK 1

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.datasets import load_iris

try:
    iris = load_iris()
    df = pd.DataFrame(data=iris.data, columns=iris.feature_names)
    df['species'] = iris.target
    df['species'] = df['species'].map(dict(enumerate(iris.target_names)))
    print("Dataset loaded successfully!")
except Exception as e:
    print(f"Error loading dataset: {e}")

= Dataset loaded successfully!
    

