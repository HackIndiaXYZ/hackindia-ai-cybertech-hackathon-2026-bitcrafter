# DeepScan AI 🌊🤖
### AI-Powered Underwater Marine Debris Detection

DeepScan AI is a prototype designed to help identify potential underwater marine debris from **side-scan sonar imagery**. It combines sonar-image preprocessing with YOLO-based object detection to highlight objects that may require further inspection.

The project aims to support more efficient underwater inspections and better-informed marine debris cleanup efforts.

> **Project status:** Prototype / in development. Detection performance and real-world suitability should be validated before operational use. Live mapping and underwater robotic integration are future goals, not claimed as completed features.

## 🌍 Problem Statement

Underwater debris can be difficult to locate because of limited visibility, complex sonar imagery, and the time required for manual image analysis. Debris such as abandoned fishing nets, plastic waste, and metal objects can threaten marine ecosystems.

## 💡 Our Solution

DeepScan AI processes side-scan sonar images and uses an AI-based detection workflow to help identify and visualize potential debris.

### Workflow

1. **Sonar image input** — provide side-scan sonar imagery.
2. **Image preprocessing** — apply supported preprocessing steps such as noise reduction, contrast enhancement, and image normalization.
3. **Object detection** — use a YOLO-based model to detect potential debris.
4. **Classification and visualization** — display detected objects with bounding boxes and class labels, where supported by the trained model.
5. **Inspection support** — use the results to help prioritize objects for human review.

## ✨ Key Features

- AI-assisted analysis of side-scan sonar images
- YOLO-based object detection workflow
- Visual highlighting of detected objects
- Intended categories include fishing nets, plastic waste, and metal objects, depending on model training and available labels
- Modular scope for future improvements

## 🛠️ Technology Stack

- **Python** — primary development language
- **YOLOv8 / Ultralytics** — object detection (if used in the current implementation)
- **OpenCV** — image processing
- **Deep Learning** — detection model approach

Update this section to match the exact libraries and model version used in your repository.

## 🚀 Getting Started

The exact setup depends on the code and model files included in your repository. The following is a general setup for a Python-based prototype.

### Prerequisites

- Python 3.9 or a compatible version required by your dependencies
- `pip`
- A trained YOLO model weights file, if the project uses custom-trained weights
- Side-scan sonar images for testing

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/<your-username>/<your-repository>.git
   cd <your-repository>
   ```

2. (Recommended) Create and activate a virtual environment:

   **Windows**
   ```bash
   python -m venv .venv
   .venv\Scripts\activate
   ```

   **macOS / Linux**
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

3. Install the dependencies listed in your project:

   ```bash
   pip install -r requirements.txt
   ```

   If your repository does not yet contain a `requirements.txt`, create one containing the packages your code actually uses before running this command.

### Running the Project

Run the entry-point script used by your repository. For example:

```bash
python <your-entry-file>.py
```

Replace `<your-entry-file>.py` with the actual script name. If the project uses a notebook, web app, or separate frontend/backend, follow the run instructions for that component instead.

## 📂 Suggested Repository Structure

Your actual files may differ; this is a suggested structure only.

```text
DeepScan-AI/
├── README.md
├── requirements.txt
├── data/
│   ├── input/              # Sample sonar images (if permitted to share)
│   └── README.md           # Dataset source, license, and notes
├── models/
│   └── best.pt             # Trained model weights (if available)
├── src/
│   ├── preprocess.py       # Image preprocessing
│   ├── detect.py           # Detection workflow
│   └── visualize.py        # Result visualization
├── outputs/                # Generated detection results
└── docs/                   # Project presentation and documentation
```

Do not add folders or files above to the repository unless they actually exist in your project.

## 🧪 Example Use

1. Select a side-scan sonar image.
2. Run the preprocessing and detection workflow implemented in the project.
3. Review the annotated output and predicted labels.
4. Verify detections manually before using them for any cleanup or inspection decisions.

Screenshots or sample outputs can be added here once available:

```markdown
![DeepScan AI detection example](docs/images/detection-example.png)
```

## 🔭 Future Scope

- Improve model accuracy and evaluate it on diverse sonar imagery
- Expand and validate debris categories
- Add reliable geolocation and live mapping
- Explore integration with remotely operated or autonomous underwater vehicles (ROVs/AUVs)
- Build a dashboard for monitoring and reviewing detections

## 👥 Team Bitcrafter

Developed by **Team Bitcrafter** at **Kanpur Institute of Technology**.

- Harsh
- Prachi Gupta
- Jatin Singh

## 🌱 Impact

DeepScan AI explores how AI-assisted sonar analysis could help make underwater debris inspections more efficient and support marine conservation.

## ⚠️ Limitations

- Model quality depends on training data, sonar conditions, and the trained weights used.
- A detection is a prediction, not confirmation that an object is debris.
- Exact object location requires reliable positioning data and is not guaranteed by image detection alone.
- Real-time performance, accuracy, and field readiness should be measured and validated before deployment.

## 🤝 Contributing

Suggestions and contributions are welcome. Open an issue to discuss a bug or proposed improvement before submitting a pull request.

## 📄 License

No license has been specified yet. Add a `LICENSE` file before describing this project as open source, and ensure any datasets, images, and model weights are shared in accordance with their licenses.

---

**DeepScan AI — Turning sonar images into smarter ocean monitoring.**
