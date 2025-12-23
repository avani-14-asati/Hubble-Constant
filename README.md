In this project, I cleaned a dataset of supernovae to estimate the Hubble constant, which tells us how fast the
universe is expanding.

Technologies used:
Python , Jupyter notebook, Matplotlib, Pandas, NumPy, Astropy, Scipy

Process
1. Data Cleaning:
Removed missing values and filtered redshift (zHD) using 3-sigma clipping to remove outliers.
2. Hubble Diagram:
Plotted distance modulus (MU_SH0ES) vs redshift to visualize the redshift-distance relation.
3. Model Fitting:
Used a flat ΛCDM cosmology model with numerical integration to compute theoretical distances.
Applied curve_fit to estimate best-fit values of H0
4. Age Estimation:
Calculated the age of the universe using the fitted parameters.
5. Redshift Split:
Divided the data into low-z and high-z samples to compare fitted H₀ values.
6. Residual Analysis:
Plotted residuals (observed − model) to check the model fit.
  
Observations:
1. Fitted H₀ ≈ 72.86 km/s/Mpc, slightly higher than Planck18, matching SH0ES results.
2. Estimated Age ≈ 12.25 Gyr, which is reasonable but slightly younger than Planck’s ~13.8 Gyr.
3. Low-z H₀ < High-z H₀, showing a mild trend that may hint at redshift-dependent behavior.
4. Residuals were mostly flat, indicating a good model fit.
