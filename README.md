# Speech Recognition and Audio Feature Extraction

This project demonstrates a simple speech recognition and audio feature extraction pipeline using Python. It processes audio files (e.g., `.flac`, `.wav`), extracts useful audio features like MFCC, pitch, energy, and signal-to-noise ratio (SNR), and saves them in a CSV file that can be imported into Power BI for visualization.

## 📁 File Contents

- `NM2 (2).ipynb`: Main Jupyter Notebook containing all the code for:
  - Audio loading and preprocessing
  - Feature extraction using Librosa
  - SNR estimation
  - Classification of clean/noisy audio
  - CSV file generation for Power BI

## 🔧 Requirements

Install the following Python libraries before running the notebook:

```bash
pip install librosa pandas numpy soundfile tqdm
Make sure you have ffmpeg installed and added to your system path.

🎧 Input
Audio files in .flac, .wav, or other supported formats

Folder structure should be updated in the notebook as the root directory path

📊 Output
A CSV file (audio_features_metadata_2.csv) containing:

File path

Duration

MFCC mean

Pitch mean

Energy

Estimated SNR

Clean/Noisy label

This CSV can be imported into Power BI for creating visual dashboards.

💡 Usage
Place your audio files inside a folder.

Update the root_dir variable in the notebook with the folder path.

Run all the cells.

Locate the generated audio_features_metadata_2.csv file.

Import it into Power BI to build your visualization.

📌 Note
If you are working on only a single audio file, make sure to put it in a folder and provide that folder path in the code to allow os.walk to find it.
