# Player Tracking in Sports Videos - Neural Networks Assignment

A complete computer vision system for detecting, tracking, and analyzing players in sports videos using YOLOv8 and pose estimation.

## 📁 Project Structure

```
player_tracking/
├── README.md                          # This file
├── requirements.txt                   # Python dependencies
├── setup_environment.sh               # Environment setup script
├── notebooks/
│   ├── 01_dataset_preparation.ipynb   # Video collection and preprocessing
│   ├── 02_player_detection.ipynb      # YOLOv8 player detection
│   ├── 03_keypoint_detection.ipynb    # Pose estimation
│   ├── 04_player_tracking.ipynb       # Multi-object tracking
│   └── 05_evaluation.ipynb            # Performance metrics
├── src/
│   ├── data_preparation.py            # Dataset utilities
│   ├── detection.py                   # Player detection module
│   ├── pose_estimation.py             # Keypoint detection module
│   ├── tracking.py                    # Player tracking module
│   ├── evaluation.py                  # Metrics calculation
│   └── visualization.py               # Output generation
├── data/
│   ├── videos/                        # Input videos
│   ├── frames/                        # Extracted frames
│   └── annotations/                   # Ground truth (if available)
├── outputs/
│   ├── videos/                        # Processed videos
│   ├── screenshots/                   # Sample frames
│   └── metrics/                       # Performance graphs
├── models/                            # Pre-trained weights
└── report/
    └── REPORT.md                      # Final assignment report
```

## 🚀 Quick Start

### 1. Environment Setup

```bash
# Clone or download the project
cd player_tracking

# Create virtual environment
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### 2. Download Sports Videos

Place 5-10 sports video clips (5-10 seconds each) in `data/videos/`:
- football, football, rugby, basketball, etc.
- Download from YouTube using `yt-dlp` or other sources
- Recommended: 720p or 1080p resolution

### 3. Run the Pipeline

**Option A: Use Jupyter Notebooks (Recommended for learning)**
```bash
jupyter notebook
# Open notebooks in order: 01 → 02 → 03 → 04 → 05
```

**Option B: Use Python Scripts**
```bash
# Step 1: Prepare dataset

python -m venv venv      
 .\venv\Scripts\Activate.ps1
pip install -r requirements.txt
 jupyter notebook