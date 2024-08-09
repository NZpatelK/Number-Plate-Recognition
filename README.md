# 🚗 Number Plate Recognition

This open-source project is available for everyone to use. Feel free to clone or fork it into your GitHub repository, allowing you to customize it according to your needs.

In this guide, I'll walk you through how to use the application for recognizing number plates from images, videos, or even in real-time using a webcam.

---

### 📑 Table of Contents

- [🔧 Installing Required Packages](#-installing-required-packages)
- [📂 Importing Images or Videos](#-importing-images-or-videos)
- [🖼️ Image-Based Recognition](#-image-based-recognition)
  - [🖼️ Single Image](#single-image)
  - [🖼️ All Images](#all-images)
  - [🖼️ Group of Images](#group-of-images)
- [🎥 Video-Based Recognition](#-video-based-recognition)
  - [🎥 Single Video](#single-video)
  - [🎥 All Videos](#all-videos)
  - [🎥 Group of Videos](#group-of-videos)
- [📸 Webcam-Based Recognition](#-webcam-based-recognition)
- [📁 Accessing the Results](#-accessing-the-results)

---

### 🔧 Installing Required Packages

The necessary packages are listed in the `requirements.txt` file. Please avoid modifying this file to ensure the application runs smoothly.

**To install the packages:**

1. Open your console or terminal.
2. Navigate to the project directory.
3. Run the following command:

```console
pip install -r requirements.txt
```

This command will install all the required packages as specified in the `requirements.txt` file.

---

### 📂 Importing Images or Videos

Inside the `assets` folder, there are two subfolders: `images` and `videos`. Simply place your images or videos in the corresponding folder.

---

### 🖼️ Image-Based Recognition

#### 🖼️ Single Image

To run recognition on a specific image, use the following command:

```console
python predict_modified.py source='assets/images/[your file name with extension]'
```
**Example:**
```console
python predict_modified.py source='assets/images/Cars1.png'
```

#### 🖼️ All Images

To process all images in the `images` folder:

```console
python predict_modified.py source='assets/images'
```

#### 🖼️ Group of Images

If you have a set of related images, create a subfolder within `assets/images` and store your images there. Then, run:

```console
python predict_modified.py source='assets/images/[your subfolder name]'
```
**Example:**
```console
python predict_modified.py source='assets/images/car_group1'
```

---

### 🎥 Video-Based Recognition

#### 🎥 Single Video

To run recognition on a specific video, use the following command:

```console
python predict_modified.py source='assets/videos/[your file name with extension]'
```
**Example:**
```console
python predict_modified.py source='assets/videos/Cars1.mp4'
```

#### 🎥 All Videos

To process all videos in the `videos` folder:

```console
python predict_modified.py source='assets/videos'
```

#### 🎥 Group of Videos

If you have a collection of related videos, create a subfolder within `assets/videos` and store your videos there. Then, run:

```console
python predict_modified.py source='assets/videos/[your subfolder name]'
```
**Example:**
```console
python predict_modified.py source='assets/videos/car_group1'
```

---

### 📸 Webcam-Based Recognition

To use your webcam for real-time number plate recognition:

```console
python predict_modified.py source='0'
```

---

### 📁 Accessing the Results

All processed results are automatically saved in the `results` folder. You can review your recognition outputs there.
