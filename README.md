# BoundingBox-Annotation-Tool

A lightweight image annotation tool using OpenCV for drawing bounding boxes and saving annotations in YOLO format. Ideal for preparing custom object detection datasets.

## 📌 Features

- Manual bounding box annotation using mouse.
- Save annotations in YOLO format (.txt files).
- Automatically creates directories for annotated images and labels.
- Easy navigation through image dataset.

## 🖼️ How It Works

1. Load all images from the given folder.
2. Use mouse to draw bounding boxes.
3. Press `s` to save annotations.
4. Annotations are stored in `annotated_data/images` and `annotated_data/labels` directories.

## 🎮 Controls

| Key | Action                   |
|-----|--------------------------|
| `s` | Save annotation          |
| `d` | Next image               |
| `a` | Previous image           |
| `q` | Quit annotation session  |
| `r` | Remove last bounding box |

## 🚀 Usage


python BoundingBox-Annotation-Tool.py
You will be prompted to enter the image folder path and class name.

📝 Output Format (YOLO)
Each label .txt file will contain:

php-template
Copy
Edit
<class_id> <x_center_norm> <y_center_norm> <width_norm> <height_norm>
Where all values are normalized between 0 and 1.

🧰 Requirements
Python 3.x

OpenCV

Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
📁 Folder Structure
mathematica
Copy
Edit
project/
│
├── BoundingBox-Annotation-Tool.py
├── requirements.txt
├── annotated_data/
│   ├── images/
│   └── labels/
📣 Notes
Class ID is auto-inferred from the class name input.

Images and annotations are saved in YOLO-compatible format for training with models like YOLOv5, YOLOv8, etc.


