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
[Kaggle Link](https://www.kaggle.com/datasets/abdullahorzan/moodify-dataset)

## Some Screenshots

## Data Visualizations 
<img width="400" alt="image" src="https://github.com/user-attachments/assets/2ece711a-1e43-4442-a326-c51b7ff15748" />
<img width="457" alt="image" src="https://github.com/user-attachments/assets/37061877-7d3d-4b6c-8e58-c00e646a39b1" />
<img width="464" alt="image" src="https://github.com/user-attachments/assets/01022aa7-d89b-4824-a663-a0811112c429" />
<img width="400" alt="image" src="https://github.com/user-attachments/assets/09675329-b8de-421b-8316-c27e77a47187" />

## WebCam
![ChatGPT Image Jul 1, 2025, 10_50_18 PM](https://github.com/user-attachments/assets/c292ad97-8194-413a-9e13-68289d925f79)
![ChatGPT Image Jul 1, 2025, 10_44_08 PM](https://github.com/user-attachments/assets/0fa963f8-5a33-44c9-92dd-00c93d9e7a39)

##  How It Works

### 1. Clone the Repository
```bash
git clone https://github.com/NahinFatima/Moodify-Music-Recommender.git
cd Moodify-Music-Recommender
```

### 2. Install Required Libraries
Make sure you have Python 3 installed. Then install the required Python packages:
```bash
pip install opencv-python deepface tensorflow pandas matplotlib seaborn numpy
 ```
 
### 3. Launch the Jupyter Notebook
```bash
jupyter notebook
```
Then open the project notebook (.ipynb file) and run all cells to start the application.

## Real-Time Mood Detection Process
1. The webcam opens and captures your face using OpenCV.
2. DeepFace analyzes the live frame to detect your dominant facial emotion.
3. The detected emotion is mapped to the mood category.
4. A relevant song is selected from the local dataset of 278k Spotify songs.
5. The song's Spotify URL is opened in your default browser.
6. A custom UI updates in real time to show:
     🎭 Current Emotion
     🎵 Mapped Mood
     📈 Animated waveform
     😀 Mood indicator visuals (emoji + color theme)

## Data Visualizations
The project includes several elegant, interactive data visualizations to explore song characteristics by mood:
- Radar Plots: Show mood-wise audio profiles across features like energy, valence, and danceability.
- Pairplots: Reveal relationships between audio features grouped by mood/emotion.
- Heatmaps: Visualize feature correlations and how they vary across different moods.
- Boxplots: Styled like equalizers to compare energy levels across moods.
- Histograms: Display the distribution of track durations by mood.
