# 🧠 Brain Tumor Segmentation using U-Net

This project implements a deep learning pipeline for segmenting brain tumors in MRI scans using the U-Net architecture. The segmentation masks highlight tumor regions, aiding medical professionals in diagnostic processes.

## 📌 Features

- U-Net architecture implemented for biomedical image segmentation
- Preprocessing of MRI brain images with resizing, normalization
- Training/validation split with real-time data augmentation
- Visualization of segmentation results and training metrics
- Evaluation using Dice coefficient and loss metrics

## 📁 Project Structure

```
brain-tumor-segmentation-u-net/
├── brain_tumer_segmentation_u_net.ipynb
├── data/
│   ├── images/
│   └── masks/
└── README.md
```

## 🚀 How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/brain-tumor-segmentation-u-net.git
cd brain-tumor-segmentation-u-net
```

### 2. Install Dependencies

```bash
pip install numpy pandas matplotlib opencv-python scikit-learn tensorflow
```

### 3. Prepare the Dataset

- Place the brain MRI images in `data/images/`
- Place corresponding binary masks in `data/masks/`

Make sure image and mask filenames match exactly.

### 4. Run the Notebook

Launch the notebook:

```bash
jupyter notebook brain_tumer_segmentation_u_net.ipynb
```

## 🧪 Dataset

You can use publicly available datasets like:

- [BRATS Dataset](https://www.med.upenn.edu/sbia/brats2018.html)
- Custom datasets with brain tumor masks

Ensure masks are in binary format where tumor regions are marked as 1.

## 🧠 Model Architecture

- **U-Net**: An encoder-decoder CNN architecture optimized for biomedical image segmentation.
- Input size: 224x224
- Output: Binary mask (tumor region vs. non-tumor)
- Loss: Binary Cross-Entropy + Dice Loss
- Optimizer: Adam

## 📊 Evaluation Metrics

- Dice Coefficient
- IoU (optional)
- Loss curve plots
- Visual comparison of predicted vs. ground truth masks

## 📈 Visualizations

- Training & validation loss plots
- Dice score curves
- Overlay of masks on MRI slices for qualitative analysis

## 📌 TODO

- [ ] Add support for multi-class segmentation
- [ ] Hyperparameter tuning automation
- [ ] Export trained model for deployment

## 📜 License

This project is open-source and available under the MIT License.
