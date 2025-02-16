# YouTube-Video-Summarizer-video_to_text-
Convert YouTube videos into concise, readable formats (PDF and DOCX) to quickly grasp the content without wasting time.
This Python script downloads audio from a YouTube video, transcribes it into text, summarizes the content, and generates professional PDF and DOCX documents. Perfect for students, professionals, and anyone who wants to save time by extracting key information from videos.

**Why Use This Tool?**

Save Time: Skip watching long videos and get straight to the key points.
Readable Formats: Get a clean, professional summary and transcript in PDF or DOCX format.
Easy to Use: Just provide the YouTube URL, and the tool does the rest.
Offline Access: Download the summary and transcript for offline reading or sharing.

**Features**

Audio Extraction: Downloads audio from any YouTube video.
Accurate Transcription: Uses OpenAI's Whisper model to convert audio into text.
Smart Summarization: Summarizes the transcript using the facebook/bart-large-cnn model.
Professional Output: Generates PDF and DOCX files with a clean, readable layout.
Temporary File Cleanup: Automatically deletes temporary files after processing.

**How It Works**

Download Audio: Extracts audio from the YouTube video and saves it as an MP3 file.
Transcribe Audio: Converts the audio into a full text transcript.
Summarize Text: Condenses the transcript into a concise summary.
Generate Documents: Creates a PDF and DOCX file containing the summary and full transcript.

**Requirements**

Python 3.7 or higher
FFmpeg (for audio extraction)
Required Python libraries (install via pip install -r requirements.txt)
Required Libraries
yt-dlp (for downloading YouTube audio)
transformers (for transcription and summarization)
reportlab (for PDF generation)
python-docx (for DOCX generation)


**Install the dependencies with:**
pip install yt-dlp transformers reportlab python-docx


**Installation**
**1.Clone the repository:**
  git clone https://github.com/your-username/youtube-to-readable.git
  cd youtube-to-readable
**2.Install the required libraries:**
  pip install -r requirements.txt
**3.**
  Ensure FFmpeg is installed and accessible in your system PATH. For Windows, you can specify the FFmpeg path in the ydl_opts dictionary in the script.


**Usage**
**Run the script:**
python youtube_to_readable.py

Enter the YouTube video URL when prompted.
The script will:

Download the audio.
Transcribe the audio into text.
Summarize the text.
Generate a PDF and DOCX file.

The output files (video_summary_.pdf and video_summary_.docx) will be saved in the current directory.

  
**Customization**

FFmpeg Path: If you're using Windows, update the ffmpeg_location in the ydl_opts dictionary to point to your FFmpeg executable.
Summarization Model: You can change the summarization model by modifying the summarizer pipeline in the summarize_text function.

**Limitations**

The script relies on external models (e.g., Whisper for transcription, BART for summarization), which may have usage limits or require an internet connection.
Large audio files may take longer to process.


**Contributing**
Contributions are welcome! If you have ideas for improvements or find any issues, feel free to open an issue or submit a pull request.



**Key Highlights:**

The main aim (converting YouTube videos into readable formats) is emphasized in the title and description.
The value proposition (saving time and providing easy-to-read summaries) is clearly stated.
The instructions are simplified and user-friendly.
