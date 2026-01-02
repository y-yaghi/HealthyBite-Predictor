## Data Access

This project uses the Open Food Facts dataset hosted on Kaggle.

The dataset is **not stored in this repository**. Instead, it is downloaded programmatically at runtime using `kagglehub`:

```python
import kagglehub
path = kagglehub.dataset_download("openfoodfacts/world-food-facts")
```
