# FoodSight AI - Indian Food Classification 🍛

![FoodSight AI Banner](https://img.shields.io/badge/FoodSight-AI-ff6b6b?style=for-the-badge&logo=fastapi)
![Render Deployment](https://img.shields.io/badge/Deployed-Render-46E3B7?style=for-the-badge&logo=render)
![IoT Powered](https://img.shields.io/badge/IoT-ESP32--CAM-orange?style=for-the-badge&logo=espressif)
![Deep Learning](https://img.shields.io/badge/AI-MobileNetV3-yellow?style=for-the-badge&logo=tensorflow)

FoodSight AI is a deep learning application capable of classifying **100 different Indian food dishes** with high accuracy. It features a modern web interface, real-time camera support, and detailed nutritional breakdown.

**🚀 [Live Demo on Render](https://food-sightai.onrender.com)**

## ✨ What's New (Review 4 Update)

-   **Flexible Portion Selection**: Input custom counts or grams/ml for hyper-accurate nutrition.
-   **Stability Hardening**: Fixed duplicate scan history bug and optimized database connections.
-   **UI Refinement**: Upgraded glassmorphism controls and polished animations.
-   **Production Guide**: Complete documentation for deploying beyond localhost.

## 🚀 Features

-   **100-Class Classification**: Identifies dishes like Butter Chicken, Masala Dosa, Biryani, and more.
-   **Dynamic Nutritional Insights**: Provides scaling calories and macros based on your custom portion size.
-   **Dietary Suitability**: Real-time advice for Veg/Non-Veg/Vegan and health precautions.
-   **Stability-First History**: Intelligent de-duplication for a clean scan timeline.
-   **Camera Support**: Real-time image capture and classification.
-   **Responsive UI**: Premium glassmorphism design that works on Desktop and Mobile.


## 📂 Documentation & Results

We have included detailed reports and visualizations of the training process:

-   **[Executive Summary](docs/REVIEW_4_EXECUTIVE_SUMMARY.md)**: High-level project overview, objectives, and technical highlights.
-   **[Review 4 Achievements](docs/REVIEW_4_ACHIEVEMENTS.md)**: Detailed status report of all implemented features.
-   **[Feature Specification](docs/FEATURE_SPECIFICATION.md)**: Complete technical specification of current and future features.
-   **[Training Journey](docs/TRAINING_JOURNEY.md)**: A narrative of how we built and refined the model.
-   **[Results & Metrics](docs/Results/REVIEW_4_RESULTS.md)**: Detailed performance analysis, confusion matrices, and F1 scores.
-   **[Visualizations](docs/Training_Graphs/)**: Loss curves, accuracy plots, and training phases.

## 🛠️ Installation

1.  Clone the repository:
    ```bash
    git clone https://github.com/yourusername/FoodSight-AI.git
    cd FoodSight-AI
    ```

2.  Create a virtual environment (optional but recommended):
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3.  Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4.  Run the application:
    ```bash
    python app.py
    ```

5.  Open your browser at `http://localhost:5000`.

## 📂 Project Structure

```
FoodSight-AI/
├── app.py                  # Flask backend (routes, auth, prediction)
├── requirements.txt        # Python dependencies
├── backend/                # Data & config modules
│   ├── nutrition_data.py   # Nutritional info for 100 classes
│   ├── dataset_config.py   # Class names & dataset stats
│   └── portion_data.py     # Portion size definitions
├── frontend/               # UI assets
│   ├── static/css/         # Stylesheets (glassmorphism theme)
│   ├── static/js/          # Client-side JavaScript
│   └── templates/          # HTML templates
├── model/                  # Trained AI model
│   └── best_model_v6_final (fine-tuned).keras
├── scripts/                # Training & utility scripts
└── docs/                   # Training journey & results
```

## 🧠 Model Details

-   **Architecture**: MobileNetV3Large (Transfer Learning + Fine-Tuning)
-   **Dataset**: 100 Classes, ~600 images per class.
-   **Accuracy**: ~91% Training, ~78% Validation (Top-3: ~94%)
## Team

| Name | Branch | Role |
|------|--------|------|
| **Tanmay** | CSE | Backend / ML |
| **Rishabh** | CSE | UI / Frontend |
| **Ishaan** | CSE | Nutrition / Dataset |
| **Mokshesh** | CSE | Documentation |
| **Moushikka** | VLSI | VLSI / Hardware |

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
