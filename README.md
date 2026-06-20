# 🏃‍♂️ Player Re-Identification in a Single Video Feed using YOLOv11 + DeepSORT

This project tracks and re-identifies players in a 15-second sports video using a fine-tuned YOLOv11 object detection model and the DeepSORT tracking algorithm. The entire workflow runs on **Google Colab**, requiring no local setup.

for the StereoVision part go to

https://github.com/aaravsingla/Sterio-Computer-Vision/tree/main/DENSE-3D-RECONSTRUCTION-main

---

## 🎯 Project Objective

- Detect all players in a short video clip.
- Assign each player a unique ID.
- Ensure the same player retains their ID, even when temporarily leaving and re-entering the frame.

This project simulates **real-time re-identification and tracking**, commonly used in sports analytics and surveillance.

---

## 🔧 Technologies Used

| Component         | Tool/Library |
|------------------|--------------|
| Object Detection | YOLOv11 (Ultralytics) |
| Multi-Object Tracking | DeepSORT |
| Environment      | Python 3 (Google Colab) |
| Video Processing | OpenCV |

---

## 📁 Files in This Repository

📦 Player-Reidentification
├── 📓 sportsCNN.ipynb # Main Google Colab notebook|
├── 📓 sportscnn.py # Main code in notebook|
├── 📄 README.md # Project overview and instructions|
├── 📄 output.avi # Project output|


---

## 🚀 How to Run (Google Colab Only)

You do **not** need to run anything locally. Just follow these steps:

### 1️⃣ Open the Colab Notebook

> 📌 Click here → [Open in Colab](https://colab.research.google.com/drive/1yZRQ4siCrN98UjT_Sf2E-NF50_Veg-KC?usp=sharing)

### 2️⃣ Upload Required Files to Google Drive

Place the following files in your Google Drive:
- `best.pt` → Fine-tuned YOLOv11 model (for detecting players)
- `15sec_input_720p.mp4` → The 15-second sports video

### 3️⃣ Follow Instructions in the Notebook

The notebook:
- Mounts your Google Drive
- Installs necessary packages
- Loads the model and video
- Performs player detection and tracking
- Saves and downloads the output video with tracking annotations

---

## 🎬 Output

The output is a video (`deepsort_output.avi`) with:
- Bounding boxes around each detected player
- Consistent player IDs across frames
- Downloadable directly from the notebook

---

## 📈 Applications

- Sports analytics
- Player substitution tracking
- Event detection in gameplay
- Heatmap and path analysis

---

## 🧠 Potential Extensions that i will work on later

- Integrate OCR to extract jersey numbers for stronger re-ID
- apply courful histograms


---

## 📄 License

This project is open source under the MIT License.  
Feel free to use, modify, or extend it.

---

## 👤 Author

Built by [Aarav Singla](https://github.com/aaravsingla)  
If you have any questions or feedback, feel free to reach out via GitHub!





