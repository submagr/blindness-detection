# APTOS 2019 Blindness Detection:
Task was to predict the severity of an input image given 3K labeled retina images. We used
various preprocessing steps (CLAHE, smoothing, blood vessels segmentation) to remove noise and variable lighting conditions using OpenCV. We experimented with various architectures (ResNet, EfficientNet) and training parameters to improve score using PyTorch. EfficientNet-B2 and TTA gave a final optimized kappa score of 0.895 and final leaderboard ranking of 1309.

### Setup
- Virtual Environment Setup and 
```python
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

- Install Data from kaggle in `data\`

- Make virtual environment compatible with Jupyter Notebook 
```python
ipython kernel install --user --name=blindness-detection
```
