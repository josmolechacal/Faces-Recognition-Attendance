# 📦 Installation & Configuration Guide  
Face Recognition Attendance System

## Prerequisites
- Python 3.9 or higher  
- Git  
- Conda (Anaconda or Miniconda)

## Clone the Project
git clone <repo-link>
cd <project-folder>

## 🐍 Conda Environment Setup
conda --version

### Create Environment
conda create -n fra_env python=3.9
conda activate fra_env

### Install Dependencies
pip install opencv-python numpy
# or
conda install -c conda-forge opencv numpy

### Using base (Not Recommended)
conda activate base
pip install opencv-python numpy

## Environment File (Recommended)
name: fra_env
channels:
  - conda-forge
dependencies:
  - python=3.9
  - opencv
  - numpy

conda env create -f environment.yml
conda activate fra_env

## Camera Configuration (iVCam)
- Install iVCam on smartphone and computer  
- Launch iVCam on both devices  
- Connect to the same network  
- Ensure virtual camera is detected  

## Network Requirements
- Same local network required  
- Avoid institutional networks  

## Test
python camera_selector.py
python test_camera.py

## Notes
- Start iVCam before running scripts  
- Verify camera index  
