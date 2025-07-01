# ☀️ FlareNet  
**Multivariate Time Series Prediction of Solar Flares via Functional Embedding and Sequence Modeling**

FlareNet is a deep learning-based system for **predicting solar flares**—violent eruptions on the Sun that can severely impact satellites, communication networks, and power infrastructure. By fusing **multivariate time series analysis** with **graph-based functional embedding** and **sequence modeling**, FlareNet captures both spatial interdependence between solar regions and their temporal dynamics. The hybrid architecture combines **GCNs** for topological feature learning and **LSTMs** for sequence modeling to enable early and reliable forecasting of space weather events.

---

![Model Architecture](https://user-images.githubusercontent.com/11091318/155829709-ad12652c-3bc8-46ff-acdb-71aa3b0ef349.png)  
*Functional graph embedding using GCN and sequential modeling using LSTM for multiscale solar flare forecasting.*

---

## 🧠 Project Structure

```bash
FlareNet/
├── data/          # Preprocessed multivariate time series datasets
├── models/        # GCN-LSTM and baseline models
├── utils/         # Helpers for data loading, batching, preprocessing
└── requirements.txt
```

- `data/`: Contains the solar flare datasets used for training and evaluation.
- `models/`: Core implementations of GCN-LSTM and other baselines.
- `utils/`: Utility scripts for preprocessing and visualization.

---

## ⚙️ Setup Instructions

### Environment

- **Python**: 3.9.7  
- **CUDA**: 11.1 (tested on Windows Server)

### 🔧 Installation Steps

1. Install Python and optionally JupyterLab.
2. Navigate to the project root directory:
   ```bash
   cd path/to/FlareNet
   ```

3. Install dependencies:
   ```bash
   pip install wheel
   pip install -r requirements.txt
   ```

4. Run the model (from within `models/` directory):
   ```bash
   python gcn_lstm_model.py
   ```

> ⚠️ Ensure dataset paths are correctly set within the model scripts if needed.

---

## 📊 Embedding Visualization (t-SNE)

To evaluate the quality of learned representations, we use **t-SNE** on the final-layer embeddings from the GCN-LSTM pipeline:

![t-SNE](https://user-images.githubusercontent.com/11091318/156713767-5c6cc63e-c77e-4c04-ad89-3194b165d70d.png)

---

## 🔍 Highlights

- Combines **graph-based spatial modeling** and **deep sequential learning**
- Explores **functional connectivity** from time series signals
- Modular codebase with extensibility for other scientific forecasting tasks
- Built-in support for **embedding visualization** and analysis

---

## 🧭 Future Directions

- Integration of **attention mechanisms** for spatial-temporal interpretability
- Exploration of **Transformer-based encoders**
- Real-time streaming inference for satellite applications

---

## 📜 License

This project is licensed under the MIT License.

---

## 📫 Contact

If you have any questions, suggestions, or feedback, please don't hesitate to open a GitHub issue or contact us via email.

