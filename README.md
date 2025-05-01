# Object Detection with YOLOv8 🚀

Welcome to this beginner-friendly Object Detection project using YOLOv8 ! This repo helps you detect objects in real-time using your webcam. It's simple, fun and perfect for getting started with computer vision ! 🎥✨


## Screenshots 📸

Check out these cool detection results !



## Prerequisites ✅

Before you dive in, make sure you have:

- 🐍 **Python 3.7+** installed
- A **webcam** connected to your device
- Basic knowledge of Python and command-line usage
- A code editor (like VS Code)

## Folder Structure 📂

Organize your project like this for smooth execution:

```
object-detection/
├── object.py               # Main script for object detection
├── yolov8n.pt              # Pre-trained YOLOv8 model file
```

## Setup Instructions 🛠️

Follow these steps to get the project up and running:

1. **Clone the Repository**\
   Clone this repo to your local machine:

   ```bash
   git clone https://github.com/your-username/object-detection-yolov8.git
   cd object-detection-yolov8
   ```

2. **Create a Virtual Environment** (Optional but recommended)\
   Set up a virtual environment to keep dependencies clean:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**\
   Install the required Python libraries:

   ```bash
   pip install ultralytics opencv-python
   ```

   - `ultralytics`: For running YOLOv8
   - `opencv-python`: For webcam access and video processing

4. **Download the YOLOv8 Model**\
   The `yolov8n.pt` model file is required. You can download it automatically when running the code, or manually from the Ultralytics YOLOv8 releases page. Place it in the project root folder.

5. **Run the Code**\
   Execute the main script to start object detection:

   ```bash
   python object.py
   ```

   - A window will pop up showing your webcam feed with detected objects highlighted !
   - Press `q` to quit the window.

## Code Explanation 📜

The `object.py` script does the following:

- Loads the YOLOv8 model (`yolov8n.pt`)
- Accesses your webcam (`source="0"`)
- Runs object detection and displays results in real-time
- Prints detection details to the console


## Troubleshooting 🛑

Encountering issues? Here’s how to fix common problems:

- **Error: "No webcam found"**
  - Ensure your webcam is connected and functional.
  - Try changing `source="0"` to `source="1"` in `object.py` if you have multiple cameras.
- **Error: "Module not found"**
  - Verify that `ultralytics` and `opencv-python` are installed (`pip list`).
  - Reinstall dependencies if needed: `pip install ultralytics opencv-python`.
- **Model file missing**
  - Ensure `yolov8n.pt` is in the project root. If missing, the script will attempt to download it automatically.
- **Window freezes or crashes**
  - Press `q` to close the window properly.
  - Check if your system has enough memory/CPU resources.
- **Low detection accuracy**
  - The `yolov8n` model is lightweight. For better accuracy, try `yolov8m.pt` or `yolov8l.pt` (larger models, slower but more accurate).

## Tips for Beginners 🌟

- Experiment with different YOLOv8 models (e.g., `yolov8s.pt`, `yolov8m.pt`) for better accuracy.
- Save detection outputs by modifying the script (e.g., add `save=True` in `model.predict`).
- Explore the Ultralytics documentation for advanced features.

## Created With ❤️ By B P ARYAAN \[ ARYAAN-DEV \]

Feel free to contribute, raise issues, or share your awesome detection results !

Happy detecting ! 🎯
