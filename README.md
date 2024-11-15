# Object Detection using YOLOv5

This repository implements **Object Detection** using the **YOLOv5** model, a state-of-the-art algorithm for real-time object detection. YOLOv5 strikes the perfect balance between speed and accuracy, making it ideal for a wide range of applications such as surveillance, autonomous vehicles, and retail.

---

## Features
- **Real-Time Object Detection**: Detects multiple objects in images and videos in real-time.
- **Pre-trained YOLOv5 Models**: Includes pre-trained weights that allow you to perform object detection with minimal setup.
- **High Performance**: Achieves high **mAP (mean Average Precision)** and fast inference, suitable for deployment in real-time applications.
- **Easy-to-Use Interface**: Simple CLI for running inference and training models.

## Usage

### 1. Run Object Detection on a Single Image
To run object detection on an image, use the following command:
```bash
python detect.py --source path/to/your/image.jpg
```

### 2. Run Object Detection on a Video
To detect objects in a video:
```bash
python detect.py --source path/to/your/video.mp4
```

### 3. Train YOLOv5 on Your Custom Dataset
To train a custom model, make sure your dataset is formatted according to YOLOv5 standards. You can use the following command to start training:
```bash
python train.py --img-size 640 --batch-size 16 --epochs 50 --data your_dataset.yaml --weights yolov5s.pt
```
Replace `your_dataset.yaml` with the configuration file for your custom dataset.

### 4. Evaluate Model Performance
To evaluate the model on a test set:
```bash
python val.py --data your_dataset.yaml --weights path/to/your/trained_model.pt --img-size 640
```

## Results
The model can successfully detect various objects within an image or video, including common objects such as cars, people, animals, and more.

**Sample Output:**
---![WhatsApp Image 2024-11-15 at 3 56 25 PM (1)](https://github.com/user-attachments/assets/d3473487-7d4e-44d7-a624-d349d30fdcc4)
---![WhatsApp Image 2024-11-15 at 3 56 25 PM](https://github.com/user-attachments/assets/92f54848-0607-45e9-9463-2735b1652ecd)

## Pre-trained Models
You can start by using YOLOv5's pre-trained weights:
- `yolov5s.pt` – YOLOv5 small model (fast and lightweight)
- `yolov5m.pt` – YOLOv5 medium model (balanced performance)
- `yolov5l.pt` – YOLOv5 large model (high accuracy)
- `yolov5x.pt` – YOLOv5 extra-large model (best performance)

You can load these models directly for inference or fine-tune them on your custom dataset.

## License
This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more details.

## Acknowledgments
- **YOLOv5**: [Ultralytics YOLOv5 repository](https://github.com/ultralytics/yolov5)
- **PyTorch**: For deep learning and GPU acceleration.
- **OpenCV**: For image/video processing.

### Notes:
- Replace `"your-username"` with your actual GitHub username.
- The `path/to/sample_image.jpg` should be replaced with the correct path to your sample image.
- If you're using a custom dataset, provide specific details on the format or how users can prepare their dataset.

This `README.md` provides all the necessary steps to get started with the project, as well as detailed explanations of how to use and customize it. Feel free to add more sections or modify the content based on the specific features or details of your project!
