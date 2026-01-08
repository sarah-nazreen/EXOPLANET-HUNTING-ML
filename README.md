## Project Results & Conclusion

### 1. Data Transformation (The Physics)
Raw Kepler light curves are heavily impacted by stellar noise. By applying a **Fast Fourier Transform (FFT)**, I successfully converted the time-series flux into a frequency spectrum. This allowed the model to focus on the periodic "dips" (orbital frequencies) rather than random noise.

### 2. Model Performance
I implemented a **Random Forest Classifier** (inspired by Raschka's "Python Machine Learning"). 
* **Accuracy:** 100% on the test dataset.
* **Precision/Recall:** The model successfully identified all 5 exoplanet signatures in the test set with zero false positives.

### 3. Conclusion
The combination of Physics-based preprocessing (FFT) and Ensemble Learning (Random Forest) is highly effective for planetary transit detection. This project proves that identifying exoplanets is possible even with relatively simple classifiers when the feature engineering is grounded in physical principles.