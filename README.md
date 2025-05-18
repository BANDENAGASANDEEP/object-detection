# 🚀 YOLOv5 Object Detection – Custom Model Inference

Welcome to this project where we showcase **real-time object detection** using a **custom-trained YOLOv5s model**. This setup uses **Pascal VOC 2007 test images** for model evaluation in a clean and modular pipeline.

---

## 📁 Project Overview

This repository demonstrates:

✅ Cloning and configuring **YOLOv5**  
✅ Modifying model settings with a custom `yaml` file  
✅ Running inference on **real-world test images**  
✅ Saving predictions for further analysis

---

## 🌐 Project Structure

```

📂 /content/drive/MyDrive/
├── yolov5/                      ← YOLOv5 source code (cloned)
├── custom\_yolov5s.yaml          ← Modified model configuration
├── custom\_yolov5s.pt            ← Trained weights
└── voc/
└── dataset\_yolo/
└── test/
└── images/          ← Pascal VOC 2007 test images (.jpg)

````

---

## 🛠️ Setup Instructions

### 1️⃣ Clone YOLOv5

```bash
git clone https://github.com/ultralytics/yolov5 /content/drive/MyDrive/yolov5
````

### 2️⃣ Install Dependencies

```bash
cd /content/drive/MyDrive/yolov5
pip install -r requirements.txt
```

---

## 🔍 Inference on Test Images

Run the model using the command below:

```bash
python detect.py \
  --weights /content/drive/MyDrive/custom_yolov5s.pt \
  --source /content/drive/MyDrive/voc/dataset_yolo/test/images \
  --conf 0.25 \
  --save-txt \
  --save-conf
```

🖼️ Results (images with bounding boxes) are saved to:

```
/content/drive/MyDrive/yolov5/runs/detect/exp/
```

---

## 📦 Dataset Information

* **Source**: [Pascal VOC 2007 Test Set](http://host.robots.ox.ac.uk/pascal/VOC/voc2007/)
* **Format**: `.jpg` images only
* **Purpose**: Testing the accuracy and performance of the custom YOLOv5s model
* **Note**: No training, validation, or annotations included – test images only!

---

## ✨ Key Features

* 🔧 Lightweight and fast detection using YOLOv5s
* 🧠 Fully customizable model config (`custom_yolov5s.yaml`)
* 📸 Clean test dataset with real-world images
* 🧪 Focus on inference and performance analysis

---

## 🖼️ Sample Output

> *![image](https://github.com/user-attachments/assets/463de181-b841-47e5-b5c0-0304db51c2cd)
*

---

## 🔗 Resources

* 📘 YOLOv5: [https://github.com/ultralytics/yolov5](https://github.com/ultralytics/yolov5)
* 📁 VOC Dataset: [http://host.robots.ox.ac.uk/pascal/VOC](http://host.robots.ox.ac.uk/pascal/VOC)

---

## 🙌 Acknowledgements

* [Ultralytics](https://github.com/ultralytics) for YOLOv5
* Pascal VOC dataset creators

---

## 📬 Contact

For questions or collaboration, feel free to reach out!

---

```

Would you like me to save this `README.md` directly into your project directory in Google Drive?
```
