# Moodify 🎧 - Emotion-Based Music Recommendation System

**Moodify** is a hybrid AI + Data Science project that recommends Spotify songs based on your real-time facial expression. 
Using DeepFace for emotion detection and a curated dataset of 278k+ labeled tracks, 
Moodify plays mood-appropriate music and visualizes audio features through elegant plots.
## Features

- 🎥 Real-time emotion detection via webcam using **DeepFace**
- 😄 Mood classification (happy, sad, energetic, calm, neutral)
- 🎶 Mood-based song recommendation from a local dataset
- 📊 Data visualizations:
  - Feature correlation heatmap
  - Radar charts for mood-wise audio signatures
  - Pairplots for feature relationships
  - Duration histograms
  - Energy boxplots styled like an equalizer

## Technologies Used

- Python 3
- OpenCV
- DeepFace
- pandas, numpy
- seaborn, matplotlib
- webbrowser
- Jupyter Notebook

## Emotion to Mood Mapping

| Emotion    | Mapped Mood |
|------------|--------------|
| happy      | happy        |
| sad        | sad          |
| angry      | calm         |
| fear       | calm         |
| surprise   | energetic    |
| disgust    | energetic    |
| neutral    | neutral      |

## Dataset

This project uses the 278k Emotion Labeled Spotify Songs from Kaggle.
Used File: 278k_labelled_uri.csv (renamed locally to mood_song.csv)
Size: ~26MB (too large to include directly)

How to Access:
Download it manually from Kaggle:
[Link Text](https://www.kaggle.com/datasets/abdullahorzan/moodify-dataset)

## Some Screenshots

## Data Visualizations 
<img width="400" alt="image" src="https://github.com/user-attachments/assets/2ece711a-1e43-4442-a326-c51b7ff15748" />
<img width="400" alt="image" src="https://github.com/user-attachments/assets/09675329-b8de-421b-8316-c27e77a47187" />

## WebCam
![ChatGPT Image Jul 1, 2025, 10_50_18 PM](https://github.com/user-attachments/assets/c292ad97-8194-413a-9e13-68289d925f79)
![ChatGPT Image Jul 1, 2025, 10_44_08 PM](https://github.com/user-attachments/assets/0fa963f8-5a33-44c9-92dd-00c93d9e7a39)
## How it works

1. Clone the Repository:
git clone https://github.com/NahinFatima/Moodify.git
cd Moodify

2. Install Required Libraries
Make sure you have the following Python packages installed:
a. opencv-python
b. deepface
c. tensorflow 
d. pandas
e. matplotlib
f. seaborn
g. numpy

3.Launch Jupyter Notebook
Open the project notebook:
jupyter notebook

4. Real-time Mood Detection Process
- Webcam opens and captures your face using OpenCV
- DeepFace analyzes the frame and detects the dominant emotion
- The emotion is mapped to a broader mood category (e.g., happy → happy, angry → calm)
- A relevant song is selected from a local Spotify-sourced CSV dataset
- The selected song’s Spotify URL is opened in your web browser
- A custom UI is updated in real-time to display:
  - Current Emotion
  - Mapped Mood
  - Animated waveform
  - Mood indicator visuals (emoji + colors)
- Data Visualization
  Several EDA charts are generated:
  - Radar plots showing mood-based audio profiles
  - Pairplots of audio features grouped by label
  - Heatmaps for feature correlation and mood relationships
  - Boxplots and histograms to explore song energy and duration

