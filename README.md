# GA-ANFIS-Optimization-for-Global-Stock-Price-Index-Forecasting
This research project implements a hybrid approach combining **Genetic Algorithms (GA)** and the **Adaptive Neuro-Fuzzy Inference System (ANFIS)** to forecast stock price indices across various global capital markets. The primary objective of this study is to demonstrate that the GA-ANFIS model exhibits high adaptability and superior accuracy compared to manual tuning methods, particularly when faced with the diverse characteristics of stock market data across different countries.

### Research Data
This study utilizes three datasets representing the dynamics of capital markets in different economic regions. The data consists of Daily Closing Prices for the following indices:

1. **NASDAQ Composite (^IXIC)**: This dataset represents the performance of the United States stock market, specifically focusing on the technology and growth sectors. The data was collected over a comprehensive timeframe to capture significant global market volatility.

2. **Euro Stoxx 50 (^STOXX50E)**: This dataset includes 50 blue-chip stocks from countries within the Eurozone. Utilizing this data aims to test the model's performance against the stability of advanced economic markets in Europe during the same observation period.

3. **Jakarta Stock Exchange Composite (JKSE / IHSG)**: This dataset represents the Indonesian capital market (Emerging Market). The focus here is to observe how well the model adapts to the high volatility often found in the stock markets of developing nations.

*Note: All datasets cover an observation range from January 2010 to September 2025 to ensure consistency across the training and testing phases.*

### Model Description: GA-ANFIS
The model developed in this project integrates the strengths of fuzzy logic systems and artificial neural networks which automatically optimized through an evolutionary algorithm. The implementation utilizes the Adaptive Neuro-Fuzzy Inference System (ANFIS) architecture as the underlying framework to map inputs to outputs based on fuzzy membership functions. A significant challenge in conventional ANFIS is determining the optimal parameters for Membership Functions and consequent parameters, which are often difficult to tune manually. To address this, a Genetic Algorithm (GA) is integrated to search for the most effective parameters through selection, crossover, and mutation processes. This allows the model to independently adjust its fuzzy rules based on the unique characteristics of each index, whether it is the highly volatile NASDAQ or the trend-specific IHSG. While the GA-ANFIS optimization process requires substantial computational time exceeding 11 hours to reach convergence, this cost is justified by the significant increase in accuracy compared to standard methods. The experimental results indicate that this model is highly adaptive and efficient for financial practitioners who require a precise multi-index forecasting tool without the need for repetitive manual parameter tuning.

### System Requirements
To run this notebook, please ensure the following libraries are installed and the custom ANFIS library is properly configured:

* **Pandas**: For data manipulation and analysis.

`pip install pandas`


* **NumPy**: For numerical computations.

` pip install numpy`


* **Matplotlib**: For data visualization.

`pip install matplotlib`


* **Scikit-Learn**: For evaluation metrics and data preprocessing.

`pip install scikit-learn`


* **ANFIS Library**: This project uses a specific ANFIS implementation. You must download the library files from the link below and include them in your project directory:

  * **Download Link**: [ANFIS Library Source](https://drive.google.com/drive/folders/1_aqPTvUHdmOlsX04v8EUGVr2CJfSUcyM?usp=sharing)
