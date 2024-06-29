# Employee Status Detection using YOLOv8

This project aims to detect the working and non-working status of employees using the YOLOv8 object detection model. The model is trained to classify employees into two categories: working and not working.


## Getting Started

1. Clone the repository:

    ```bash
    git clone https://github.com/0shazil0/employee-status-detection.git
    cd employee-status-detection
    ```

2. Create a virtual environment and activate it:

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

### Running the Model on Set of Images

- To run the model on a set of images, use the following command:

```bash
python detect.py --source path/to/your/images --weights path/to/your/yolov8/weights --conf 0.80
```
- Replace path/to/your/images with the directory containing the images you want to process and path/to/your/yolov8/weights with the path to your trained YOLOv8 model weights.

### Running the Model on Video
- To run the model on a video file:

```bash
python detect.py --source path/to/your/video.mp4 --weights path/to/your/yolov8/weights --conf 0.80
```

### Running the Model on Webcam
- To run the model on a webcam feed:
```bash
python detect.py --source 0 --weights path/to/your/yolov8/weights --conf 0.80
```


## Results

<video controls src="[Test_Video-1.mp4](https://github.com/0shazil0/detecting-working-status/blob/main/Test_Video.mp4)" title="Title"></video>