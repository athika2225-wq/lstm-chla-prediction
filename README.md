# lstm-chla-prediction
LSTM-based time-series model to predict chlorophyll-a (Chl-a) using multivariate oceanographic data (SST anomaly, nutrients, salinity, currents). Captures temporal patterns and nonlinear relationships. Evaluated using MAE, RMSE, and R², showing strong predictive performance.
This project focuses on predicting chlorophyll-a (Chl-a) concentration in marine environments using a Long Short-Term Memory (LSTM) deep learning model. Chlorophyll-a is a key indicator of phytoplankton biomass and plays a crucial role in understanding ocean health, carbon cycles, and marine ecosystems.
The dataset consists of multiple oceanographic variables such as sea surface temperature anomaly, salinity, dissolved oxygen (O₂), nutrients (NO₃, PO₄, silicate), iron (Fe), pH, and ocean currents (uo, vo, wo) collected over time across specific geographic coordinates. These features are combined into a unified dataset and preprocessed by handling missing values, scaling, and structuring into sequential time-series inputs suitable for LSTM.

The model leverages the temporal dependencies in oceanographic data to learn patterns influencing chlorophyll concentration. A sequence-based input pipeline is constructed where past observations are used to predict future Chl-a levels. The architecture includes stacked LSTM layers followed by dense layers, optimized using appropriate loss functions and regularization techniques to improve generalization.

Model performance is evaluated using metrics such as Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R² score, both in original and transformed scales. The model demonstrates strong predictive capability, capturing non-linear relationships and temporal dynamics effectively.

The implementation is done in Python using libraries such as TensorFlow/Keras, Pandas, NumPy, and Scikit-learn.

This work can be extended for real-time marine monitoring, harmful algal bloom prediction, and climate-related oceanographic studies.
