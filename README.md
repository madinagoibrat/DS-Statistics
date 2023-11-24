import pandas as pd
import numpy as np

full_health_data = pd.read_csv("data.csv", header=0, sep=",")

Max_Pulse= full_health_data["Glucose"]
percentile10 = np.percentile(Max_Pulse, 10)

print(percentile10)
