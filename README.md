# Auto Highlights Keywords Subtitled

![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)

## Description
This repository contains a small testing project showcasing the possibility of creating highlights using speech-to-text and keyword research for automatic video cuts.

![image](https://github.com/user-attachments/assets/5b78d7fd-a524-473a-86a1-b4ce773b7008)

## Installation
```bash
pip install git+https://github.com/m-bain/whisperx.git
pip install git+https://github.com/m1guelpf/auto-subtitle.git
```

## Usage

```python
from google.colab import drive
drive.mount("/content/drive/")

# Your existing code
# ...

# Example: Find highlight segments
keyword = 'everest'
highlight_segments = find_highlight_segments(data, keyword)

# Print the highlight segments
for segment in highlight_segments:
    print(f"Start: {segment['start']}, End: {segment['end']}, Text: {segment['text']}, Index: {segment['index']}")
```

The goal is to extract an important keyword prononced in the video, to get a clip from this one.

Feel free to contribute or open issues!


