# Parking Space Detection System 🚗🅿️

## Overview

This project utilizes advanced computer vision techniques to detect and monitor available parking spaces in real-time using video footage. The system provides an intelligent solution for parking space management by dynamically identifying and highlighting occupied and free parking spots.

## 🌟 Features

- **Real-time Parking Space Detection**: Analyze video input to identify parking space availability
- **Adaptive Processing**: Dynamic thresholding that adjusts to varying lighting and environmental conditions
- **Interactive Parameter Tuning**: Customizable GUI with trackbars for fine-tuning detection parameters
- **Persistent Space Mapping**: Store manually defined parking space positions using `pickle`
- **Visual Feedback**: Color-coded display of parking space status (green for available, red for occupied)

## 🛠 Technical Overview

### How It Works

1. **Manual Parking Space Setup**
   - Manually select and mark parking space positions in the initial video frame
   - Positions are stored persistently for consistent tracking

2. **Real-Time Video Processing**
   - Process each video frame to determine parking spot occupancy
   - Apply computer vision algorithms to detect changes in parking spaces

3. **Visual Output**
   - Display processed frames with real-time parking space status
   - Show the count of available parking spaces
   - Provide immediate visual feedback on parking lot conditions

## 📸 Visual Demonstration

### Input Frame (Before Detection)
![Input Frame](https://github.com/user-attachments/assets/629a9d30-a4fa-422a-82bc-1066420cb01b)
*Raw input frame from the video before parking space detection*

### Output Frame (After Detection)
![Output Frame](https://github.com/user-attachments/assets/b8d7e201-6b67-4646-ac05-05d540833249)
*Processed frame showing detected parking spaces with color-coded occupancy status*

## 🚀 Getting Started

### Prerequisites

- Python 3.7+
- pip package manager

### Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/parking-space-detection.git
   cd parking-space-detection
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

   Required dependencies:
   - OpenCV (`opencv-python`)
   - NumPy
   - CVZone
   - Pickle

### Usage

1. Ensure you have the following files in your project directory:
   - `main.py`: Primary script for parking space detection
   - `carPark.mp4`: Video input for processing
   - `CarParkPos`: Binary file storing parking space positions
   - `carParkImg.png`: Reference image for parking space selection

2. Run the Detection Script
   ```bash
   python main.py
   ```

3. **Interaction**
   - When the program launches, it will load the video
   - Click on the frame to manually select and define parking spaces
   - Watch real-time updates of parking space availability

## 📂 Project Structure

```
parking-space-detection/
│
├── main.py               # Main detection script
├── CarParkPos            # Parking space positions (binary)
├── carParkImg.png        # Reference image for space selection
├── carPark.mp4           # Example video input
└── images/               # Screenshots and visual documentation
```


## 🙌 Acknowledgments

- OpenCV Community
- Computer Vision Research
