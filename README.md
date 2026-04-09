# EcoSort Vision

EcoSort Vision is a desktop ANN + computer vision project with a GUI that supports **SDG 12: Responsible Consumption and Production**.

The app helps classify waste into three practical categories:

- `recyclable`
- `organic`
- `landfill`

It combines:

- OpenCV preprocessing and feature extraction
- A feed-forward artificial neural network using `MLPClassifier`
- A Tkinter GUI for dataset generation, model training, and image prediction

## Why this supports SDG

Waste sorting is one of the simplest behavior changes that improves recycling quality, reduces contamination, and supports more responsible consumption systems.

## Features

- Generate a built-in demo dataset
- Train an ANN from the GUI
- Upload an image and classify it
- See confidence scores for all classes
- Get an SDG-focused action message after prediction

## Project structure

```text
app.py
requirements.txt
src/ecosort/data.py
src/ecosort/model.py
src/ecosort/gui.py
```

## Setup

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
pip install -r requirements.txt
python app.py
```

## How to use

1. Open the app.
2. Click **Generate Demo Dataset** to create sample training images in `data/demo_dataset`.
3. Click **Train Model**.
4. Use **Browse Image** to test a waste image.

You can also point the app at your own dataset folder if it uses this structure:

```text
your_dataset/
  recyclable/
  organic/
  landfill/
```

## Notes

- The demo dataset is synthetic, so it is meant for showcasing the workflow rather than production use.
- For better real-world accuracy, replace the demo data with photos from your own waste-sorting dataset.
