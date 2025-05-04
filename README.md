# 💵 Cambodian Currency Recognition with YOLOv8

This project uses the YOLOv8 object detection model to recognize Cambodian banknotes from images. The model is trained on labeled datasets of 7 denominations: 100 Riel, 500 Riel, 1000 Riel, 5000 Riel, 10000 Riel, 20000 Riel, and 50000 Riel.

## 📂 Folder Structure

```
currency_detection_yolov8/
├── data/               # Dataset (images + labels)
├── notebooks/          # Colab training notebook
├── predictions/        # Model outputs and test images
├── runs/               # YOLOv8 run artifacts
├── scripts/            # Any custom scripts (optional)
├── README.md
└── requirements.txt
```

## 🧪 Model Training (YOLOv8)

You can use the Colab notebook under `notebooks/` to:
- Install and load YOLOv8
- Train with custom banknote data
- Validate and calculate metrics (mAP, precision, recall)
- Run predictions on test images

## 🧾 Dataset Format

This project uses the [YOLO format](https://docs.ultralytics.com/datasets/detect/) with `data.yaml` inside the `data/` folder.

## 🧠 Model Info
- Base: YOLOv8n (Nano) for lightweight detection
- Trained on: 7 Cambodian currency classes
- Input Size: 640x640
- Output: Detected denomination with bounding boxes

## 🔧 Requirements

```bash
pip install -r requirements.txt
```

## 📈 Results

Model achieved high accuracy with mAP50 > 0.95 on validation images.

## 🧊 Credits

- Dataset created, Train/Test Split, Preprocessing, and Augmentation using Roboflow
- Trained and tested using Ultralytics YOLOv8
