Pattern Recognition using Machine Learning and ESP-EYE 32 Hardware Module
DeepVisionEdge

Explore the power of on-device AI with this ESP-EYE 32 object recognition system. Leveraging deep neural networks and Edge Impulse, this project demonstrates efficient and accurate pattern recognition for embedded applications.

🚀 Overview

DeepVisionEdge is a project that demonstrates efficient and accurate pattern recognition using the ESP-EYE 32 module. Leveraging deep neural networks and Edge Impulse, this project achieves high-accuracy detection of objects like keys, mobile phones, and bottles—directly on the edge.

🌟 Key Features

On-Device AI: Real-time object recognition without cloud processing

Deep Neural Networks: Optimized for embedded deployment

Edge Impulse Integration: Streamlined training & deployment

High Accuracy: ~89% accuracy in testing

ESP-EYE 32 Optimized: Tailored for Espressif’s hardware

🛠️ Technologies Used

ESP-EYE 32 (ESP32 + Camera)

Edge Impulse

Python / Node.js

ESP Tool

TensorFlow Lite (TFLite)

📂 Project Structure
DeepVisionEdge/
├── dataset/                   # Captured and labeled images
│   ├── key/
│   ├── mobile_phone/
│   ├── bottle/
├── models/                    # TFLite models from Edge Impulse
│   ├── esp32_model.tflite
├── scripts/                   # Python/Node.js scripts + ESP32 code
│   ├── data_organization.py
│   ├── esp32_inference.c
├── documentation/
│   ├── setup_instructions.md
│   ├── results.md
├── README.md
├── LICENSE

🚀 Getting Started
1. Prerequisites

ESP-EYE 32 module

ESP-IDF or Arduino IDE

Edge Impulse account

Python 3.x or Node.js

ESP Tool

2. Setup Instructions
Clone the Repository
git clone https://github.com/YOUR_USERNAME/DeepVisionEdge.git
cd DeepVisionEdge

Prepare Your Dataset

Capture 300 images (100 per class)

Store them in:

dataset/key
dataset/mobile_phone
dataset/bottle

Edge Impulse Setup

Log in → create a project

Upload dataset

Label images

Create Impulse (processing + learning blocks)

Train using MobileNetV2 transfer learning

Test in “Live Classification”

Go to Deployment → ESP32

Download .zip

Move esp32_model.tflite → models/

ESP-EYE 32 Deployment

Install ESP-IDF or Arduino IDE

Use code from scripts/esp32_inference.c

Include the .tflite model

Build and flash using ESP Tool

View results on Serial Monitor

3. Running and Testing

Power ESP-EYE 32

Show objects (key / phone / bottle) to camera

View predictions in real-time on Serial Monitor

📈 Results

Accuracy: ~89%

Latency: Very low, real-time inference

Detailed metrics in documentation/results.md

🤝 Contributing

Pull requests and issues are welcome.

📄 License

MIT License (see LICENSE file)

📬 Contact

For queries, feel free to reach out.
