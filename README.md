# License Plate Recognition and Detection

A Python-based Automatic Number Plate Recognition (ANPR) system that uses computer vision and machine learning techniques to detect and recognize license plates in images.

## Overview

This project addresses the time-consuming process of manual license plate authentication by implementing an automated detection and recognition system. Using the KNN (K-Nearest Neighbors) algorithm and computer vision techniques, the system can efficiently process and identify license plates from images.

### Key Benefits
- Reduces registration time from 30 seconds to 6 seconds
- Automates manual vehicle authentication processes
- Suitable for stationary vehicle identification
- Assists in vehicle surveillance and registration

### Applications
- Detection of stolen vehicles
- Prevention of car smuggling
- Validation of license plates
- Traffic rule violation monitoring
- Vehicle identification in accidents
- Security and surveillance

## System Requirements

### Hardware Requirements
- 64-bit processor
- Sufficient processing power for image analysis
- Camera device for image capture

### Software Requirements
- Windows XP or higher
- Python 3.x
- Python IDLE (recommended)

### Dependencies
- OpenCV (cv2)
- NumPy
- Mathematics library (math)

## Project Structure

```
license-plate-recognition-and-detection/
├── DetectChars.py          # Character detection and recognition
├── DetectPlates.py         # License plate detection in images
├── Main.py                 # Main program execution
├── PossibleChar.py         # Character candidate class definition
├── classifications.txt     # KNN training data (classifications)
├── flattened_images.txt   # KNN training data (flattened images)
└── test_img.png           # Sample test image
```

## System Architecture

The system follows a modular architecture with the following flow:
1. **Image Input Processing**
   - Original image capture
   - Conversion to grayscale
   - Threshold image generation

2. **Plate Detection**
   - Possible character identification
   - Matching character list generation
   - Plate region extraction

3. **Character Recognition**
   - Preprocessing of plate region
   - Character segmentation
   - KNN-based recognition
   - Result validation and output

## Installation

1. Clone the repository:
```bash
git clone https://github.com/AishwaryaBhargava/license-plate-recognition-and-detection.git
```

2. Install required dependencies:
```bash
pip install opencv-python numpy
```

## Usage

1. Ensure your input image meets these requirements:
   - Clear, non-blurry image
   - Stationary vehicle
   - Visible license plate

2. Place your test image in the project directory as `test_img.png`

3. Run the main program:
```bash
python Main.py
```

## Detailed Methodology

The system employs an Object-Oriented Development methodology, following these steps:

1. **Image Capture and Preprocessing**
   - Convert to grayscale
   - Apply thresholding
   - Enhance image quality

2. **Contour Detection**
   - Identify possible characters
   - Generate character vectors
   - Filter potential matches

3. **Plate Recognition**
   - Shortlist matching character vectors
   - Identify potential plate regions
   - Convert plates to grayscale and threshold

4. **Character Recognition**
   - Remove overlapping characters
   - Apply KNN algorithm
   - Extract final plate text

5. **Result Generation**
   - Print recognized characters
   - Save annotated image

## Features

### Functional Capabilities
- Image processing and character extraction
- Database training capability
- Clear image processing
- Automatic plate detection and recognition

### Non-Functional Characteristics
- High reliability
- Easy accessibility
- Efficient resource usage
- Scalable architecture
- User-friendly interface

## Future Scope

- Mobile device support (iOS, Android, tablets)
- Enhanced blurry image processing
- Moving vehicle recognition
- Detailed plate information extraction
- Extended device compatibility
- Improved image quality tolerance

## Limitations

- Requires clear, non-blurry images
- Limited to stationary vehicles
- Hardware-dependent fault tolerance
- Basic error handling during execution

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
