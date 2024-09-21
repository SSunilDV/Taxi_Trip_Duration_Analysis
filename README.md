## Dataset
Utilized the **New York City Taxi Trip Duration** dataset [available on Kaggle](https://www.kaggle.com/competitions/nyc-taxi-trip-duration/data). This dataset contains information on taxi trips in New York City over a specific period, with features such as pickup time, drop-off time, trip duration, passenger count, and geographical coordinates.

## Tasks

1. **Data Pre-processing**:

    For the first part, worked with a subset of the dataset containing 100,000 randomly sampled rows. Used the last 4 digits of your student ID as the random seed to ensure consistency. Used the following code to load the dataset and perform the sampling:

    ```python
    import pandas as pd
    import numpy as np

    # Load the dataset
    df = pd.read_csv('train.csv')

    # Set the random seed
    np.random.seed(1234)

    # Sample 100,000 rows
    df = df.sample(n=100000)
    ```

    With the samples available, performed some preliminary analysis to understand the data. Some suggestions are
    - Provide summary statistics for the dataset.
    - Check the data types of the features.
    - Handle missing or erroneous data.
    - Convert categorical data to numerical values where necessary.
    - Normalize or standardize numerical features if required.
    - Look for errors or outliers in the data.

2. **Discovering Relationships**:
   - Employed correlation analysis to discover relationships between different features (`pandas` supports this with `corr`).
   - Applied regression analysis to identify significant predictors for trip duration.
   - Explored the possibility of creating new features that might be relevant for analysis.


3. **Data Visualization**:
   - Created visualizations to represent the distribution of key features.
   - Visualized the relationship between different features and the trip duration.
   - Employed geographic visualizations to represent pickup and drop-off locations.


4. **Algorithm and Data Structure Efficiency**:
   - Justifed the choice of data structure (from arrays, stacks, queues, linked lists, and hash tables) to store the data for each of the following scenarios:
        - The dataset sorted and viewed in ascending order of trip duration. New data added to the dataset frequently, where these new trips should show up at the end of the sorted list.
        - A new field is added to the data representing the passenger's phone number. It will be used to quickly filter out the trips made by a specific passenger.

5. **Final Analysis**:
    
    Based on analysis from tasks 1-4, discussed which factors might have the greatest impact on trip duration. Provided recommendations for a company that is looking to optimize the trip duration.
