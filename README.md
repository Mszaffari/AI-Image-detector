# AI Image Detector

A sophisticated web application that analyzes and detects AI-generated images using advanced deep learning models. Built with Streamlit for an intuitive user experience, this tool leverages state-of-the-art neural network architectures to provide accurate image authenticity analysis.

## ✨ Features

- **AI-Generated Image Detection** - Identify artificially created or synthesized images
- **Multiple Format Support** - Works with JPG, JPEG, and PNG images
- **Real-Time Analysis** - Instant results with detailed confidence scores
- **Intuitive Interface** - Clean, user-friendly web-based interface
- **Advanced Models** - Powered by EfficientNet and other cutting-edge architectures
- **Clear Visualization** - Color-coded results for quick interpretation

## 🛠️ Tech Stack

- **Python** - Core programming language
- **Streamlit** - Web application framework
- **PyTorch** - Deep learning framework
- **PIL** - Image processing
- **BlazeFace** - Lightweight face detection
- **EfficientNet** - Efficient neural network architecture

## 📋 Prerequisites

Ensure you have the following installed:

- Python 3.7 or higher
- PyTorch
- Streamlit
- Pillow (PIL)
- SciPy

## 🚀 Installation

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd AI-Image-detector
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Download model weights:**
   - BlazeFace weights: `blazeface/blazeface.pth`
   - Anchor file: `blazeface/anchors.npy`

## 💻 Usage

1. **Start the application:**
   ```bash
   streamlit run App.py
   ```

2. **Open in browser:**
   Navigate to `http://localhost:8501`

3. **Upload and analyze:**
   - Select an image file
   - Click "Analyze Image"
   - View instant results

4. **Results interpretation:**
   - 🟢 **Green** - Authentic/Natural image
   - 🔴 **Red** - AI-Generated image

## 📁 Project Structure

```
├── App.py                  # Main application entry point
├── api.py                  # API and image processing
├── image.py                # Image analysis and inference
├── blazeface/              # BlazeFace model files
└── architectures/          # Neural network definitions
```

## 🧠 Supported Models

The application utilizes several advanced architectures:

- EfficientNetB4
- EfficientNetB4ST
- EfficientNetAutoAttB4
- EfficientNetAutoAttB4ST
- Xception

## 📊 Training Datasets

Models can be trained on standard benchmarks:
- DFDC (Deep Fake Detection Challenge)
- FFPP (FaceForensics++)

## ⚙️ Configuration

- **Default confidence threshold:** 0.5
- **Temporary storage:** `uploads/` directory
- **Processing time:** Varies based on image size and hardware

## 🛡️ Error Handling

The application includes robust error handling for:
- Invalid file formats
- Processing errors
- Model inference issues
- File system operations

## 🤝 Contributing

We welcome contributions! To get started:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit changes: `git commit -m 'Add your feature'`
4. Push to branch: `git push origin feature/your-feature`
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

**Note:** This tool is designed for research and educational purposes. Always verify results and use responsibly.