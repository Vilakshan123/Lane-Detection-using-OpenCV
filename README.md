# Lane Detection using OpenCV

A real-time lane detection system implemented using OpenCV and Hough Transform for video processing.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Implementation Details](#implementation-details)
- [Results](#results)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction

This project demonstrates a lane detection system using OpenCV. It applies edge detection and Hough Transform techniques to identify lane markings in video frames. The processed video is saved with detected lanes highlighted.

## Features

- Real-time lane detection
- Canny edge detection for feature extraction
- Region of Interest (ROI) selection
- Hough Line Transform for lane marking detection
- Frame-by-frame video processing

## Requirements

- Python 3.x
- OpenCV (`cv2`)
- NumPy
- Matplotlib (for visualization, optional)

## Installation

1. Clone this repository:
   ```sh
   git clone [https://github.com/your-username/lane-detection-opencv.git](https://github.com/Vilakshan123/Lane-Detection-using-OpenCV.git)
   cd Lane-Detection-using-OpenCV
   ```
2. Install dependencies:
   ```sh
   pip install opencv-python numpy matplotlib
   ```

## Usage

1. Place your video file in the project directory.
2. Update the video path in `cap = cv2.VideoCapture("your_video.mp4")`.
3. Run the script:
   ```sh
   python lane_detection.py
   ```
4. The processed video with detected lanes will be saved as `lane_detection.avi`.

## Implementation Details

### 1. **Region of Interest (ROI) Selection**
   A mask is created to focus on the area of interest (lanes) while ignoring unnecessary regions.

### 2. **Edge Detection**
   - Converts the image to grayscale.
   - Uses the Canny edge detector to detect lane edges.

### 3. **Hough Line Transform**
   - Detects straight lines corresponding to lane markings.
   - Draws lines on the original frame.

## Results

The output video displays detected lanes highlighted in green.

## Troubleshooting

- If no lanes are detected, try adjusting the Canny edge thresholds in `cv2.Canny(gray_img, low, high)`.
- Modify the ROI selection to better suit different road conditions.
- Ensure the video file path is correct.

## Contributing

Contributions are welcome! Feel free to fork the repository and submit pull requests.

## License

This project is licensed under the MIT License.

## Contact

For any queries, reach out at [your.email@example.com](mailto:vilakshanpanchal6@gmail.com).
