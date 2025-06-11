# 💪 Push-Up Counter App using Streamlit

This Streamlit app automatically detects and counts push-ups from an uploaded video using **MediaPipe Pose estimation** and **OpenCV**. It also overlays angles and count information on the video and exports the result as an `.mp4` (H.264) file for download.

---

## 📦 Features

- 📤 Upload any push-up video (`.mp4`, `.mov`, `.avi`)
- 🧠 Detect push-up motion using elbow joint angles
- 🔁 Show real-time progress and estimated time remaining
- 📊 Overlay count and angle in top-right of video
- 🎥 Export processed video in **H.264 (.mp4)** format
- ⬇️ Download final video with overlays

---

## 📸 Example Output

![Result](result.gif)

---

## 🚀 Getting Started

### 1. Clone the Repo

```bash
git clone https://github.com/yourusername/pushup-counter-app.git
cd pushup-counter-app
```

### 2. Install Requirements

```bash
pip install -r requirements.txt
```

### 3. Run the App

```bash
streamlit run app.py
```

### 📁 File Structure

```bash
pushup-counter-app/
├── app.py               # Main Streamlit app
├── requirements.txt     # Dependencies
├── result.gif           # Output GIF
└── README.md            # Project readme
```

## ✅ Requirements

* Python 3.8+

* streamlit

* opencv-contrib-python

* mediapipe

* numpy


## ⚙️ How it Works
1. Extracts pose landmarks using `MediaPipe`.

2. Calculates elbow joint angle.

3. Detects push-up motion based on elbow angle range.

4. Overlays count and angle on each video frame.

5. Exports a final video using OpenCV's `VideoWriter`.


## 📥 Output
* `pushups_result.mp4` (available via download button in the app)
