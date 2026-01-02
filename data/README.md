## Data Access

This project uses the Open Food Facts dataset hosted on Kaggle.

The dataset is **not stored in this repository**. Instead, it is downloaded programmatically at runtime using `kagglehub`:

```python
import kagglehub
path = kagglehub.dataset_download("openfoodfacts/world-food-facts")
```
All preprocessing, feature engineering, and modeling are performed directly on the downloaded data within the notebooks. No intermediate datasets were saved to disk.
