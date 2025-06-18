## Hybrid Keylogger Detection System (Memory-Resident)

This project presents a hybrid detection system for **stealthy memory-resident keyloggers**, combining **memory forensics** and **deep learning** techniques. It includes a GUI-based tool for analyzing `.raw` or `.csv` memory dumps using **Volatility plugins**, **CNN**, and **LSTM** models.

## 🚀 Features

- 📁 Upload `.csv` or `.raw` memory files (or acquire live memory)
- 🧩 Select Volatility plugins (pslist, dlllist, malfind, etc.)
- 🧠 Analyze memory dumps using trained CNN and LSTM models
- 📊 Model training and evaluation
- 🪟 GUI built with Tkinter
- 💾 Outputs saved to structured folders
- ✅ Supports live memory capture with `winpmem`

---

## 📦 Requirements

- Python 3.8+
- TensorFlow / Keras
- OpenCV
- Pandas, NumPy, Matplotlib, Scikit-learn
- Volatility 2.6
- Tkinter (comes pre-installed with Python)
- Windows OS (for live memory capture support)

Install dependencies:

```bash
pip install -r requirements.txt
````

> If `requirements.txt` is not provided, manually install:

```bash
pip install tensorflow pandas numpy opencv-python scikit-learn matplotlib
```

---

## 🖥️ How to Use

1. **Run `main.py`**
   Launches the GUI.

```bash
python main.py
```

2. **Upload or capture memory**
   Upload a `.raw` or `.csv` file, or capture live memory using `winpmem_mini_x64.exe`.

3. **Select plugins**
   Choose the Volatility plugins to extract forensic features.

4. **Analyse**
   Run detection using CNN + LSTM models.

5. **Train Models (Optional)**
   Click “Train Now” to train models from scratch.

---

## 🧪 Project Structure

```
keylogger_system/
│
├── main.py                   # Main GUI controller
├── volatility_wrapper.py     # Volatility plugin execution
├── preprocessing.py          # Data preprocessing
├── train_model.py            # Training CNN & LSTM
├── evaluate_model.py         # Evaluation metrics
├── models/                   # Saved Keras models (.h5)
├── data/
│   ├── csv/                  # Extracted features
│   ├── images/               # Grayscale images for CNN
├── outputs/                  # Plugin outputs
├── winpmem_mini_x64.exe      # Live memory capture
├── volatility-2.6.standalone.exe
```

---

## 📚 Research Context

This system was developed as part of a final-year research project titled:

**"Deep Learning in Memory Forensics for Stealthy Keylogger Detection"**
By Maliny A/P Thanaraj, 2025
Supervised by Dr. Palanichamy Naveen
Multimedia University (MMU), Cyberjaya

---

## ⚠️ Disclaimer

This tool is intended for academic and research use only. Use responsibly and ethically.

---

## 📬 Contact

For questions, feel free to reach out via GitHub issues or:

📧 [malinythanaraj27@gmail.com](mailto:malinythanaraj27@gmail.com)

```

