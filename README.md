# 🍓 FruVeg-EdgeNet

## 🌟 Overview
FruVeg-EdgeNet is an edge AI-powered solution designed for fruit and vegetable classification, specifically tailored for visually impaired users. It integrates a camera, I2S speaker, and SD card storage, running on the ESP32-S3 microcontroller. The system supports on-device model switching, local dashboards, and firmware updates via SD card or internet OTA.

## 🛠️ Features

### 🟢 Hardware Setup
- 🕶️ **Blind Glass with Camera:** Captures images for classification.
- 🧠 **ESP32-S3:** The core microcontroller, capable of running AI models.
- 🔊 **I2S Speaker:** Provides voice feedback for recognized items.
- 💾 **SD Card Storage:** Stores models, firmware updates, and content.

### 🧩 Model Support

#### 📸 Model A: Custom 96x96 CNN (Optimized with Edge-Impulse MLoPS Int 8)
- ✅ **Training Accuracy:** 99.15%
- ✅ **Validation Accuracy:** 98.55%
- ✅ **Test Accuracy:** 98.43%
- ⚡ **Latency:** 1.732 sec
- 🗃️ **RAM Usage:** 250.5 KB
- 🏷️ **Flash Usage:** 139.1 KB
- 📊 **Model Accuracy:** 98.6%
- 🔔 **Loss:** 0.05
- 📈 **Area Under ROC Curve:** 1.00
- 🏅 **Weighted Average Precision:** 0.99
- 🏅 **Weighted Average Recall:** 0.99
- 🏅 **Weighted Average F1 Score:** 0.99

#### 🚀 Model B: Fine-tuned MobileNetV2 (160x160, Unoptimized Float-32)
- ✅ **Training Accuracy:** 99.80%
- ✅ **Validation Accuracy:** 99.28%
- ✅ **Test Accuracy:** 99.42%
- ⚡ **Latency:** 11.586 sec
- 🗃️ **RAM Usage:** 1.1 MB
- 🏷️ **Flash Usage:** 2.3 MB
- 📊 **Model Accuracy:** 99.4%
- 🔔 **Loss:** 0.02
- 📈 **Area Under ROC Curve:** 1.00
- 🏅 **Weighted Average Precision:** 0.99
- 🏅 **Weighted Average Recall:** 0.99
- 🏅 **Weighted Average F1 Score:** 0.99

### 🔧 Model and Firmware Updates
- 📂 **SD Card OTA Updates:** Swap between models and firmware stored on the SD card.
- 🌐 **Internet OTA Updates:** Directly download new models or firmware over Wi-Fi.

### 📊 Local Dashboard
- 🖥️ A built-in local dashboard for managing models, viewing classification results, and updating content.

### 📚 Content Management
- 🧠 Scientific names, nutritional benefits, and other useful content are fetched via OTA and stored locally for offline access.

### ⚡ Fully On-Device Classification
- ❌ No external web server is required — everything runs directly on the ESP32.

## 📦 Installation
1. 🛠️ **Hardware Assembly:** Connect the camera, I2S speaker, and SD card to the ESP32-S3.
2. 🔧 **Firmware Upload:** Flash the initial firmware using the Arduino IDE or ESP-IDF.
3. 📂 **Model Deployment:** Copy trained models and firmware updates to the SD card or push them via OTA.
4. 📡 **Wi-Fi Setup:** Configure Wi-Fi for internet-based updates.

## 🚀 Usage
1. 🔋 **Power On:** Turn on the device.
2. 📸 **Capture & Classify:** The camera captures an image, and the model classifies it.
3. 🔊 **Voice Feedback:** The I2S speaker announces the classification result.
4. 📊 **Manage Models:** Use the local dashboard or OTA to update models and firmware.

## 🔮 Future Improvements
- ⚡ Real-time classification speed optimizations.
- 🧠 Support for additional ML architectures.
- 📊 Enhanced dashboard features for richer insights.

## 🤝 Contributing
Contributions are welcome! Feel free to submit pull requests or open issues for bug fixes and feature suggestions.

## 📝 License
This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

Let me know if you want me to add anything else or refine the layout! 🚀✨

