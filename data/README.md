## 📂 Data Access Instructions

This project uses publicly available SBA 7(a) loan data.

Download the dataset from:
https://data.sba.gov/en/dataset/7-a-504-foia/resource/d67d3ccb-2002-4134-a288-481b51cd3479

After downloading:

1. Place the file inside the `data/` folder
2. Rename it to: sba_raw.csv
3. Inside notebook use:

```python
from google.colab import files
uploaded = files.upload()
```
```
import pandas as pd
df = pd.read_csv("data/sba_raw.csv")
```

