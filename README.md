# Video Watermarking Script

This Python script processes video files to add both visible and invisible watermarks. The output includes two separate videos:
1. **Visible Watermarked Video**: A semi-transparent watermark is applied to selected frames.
2. **Invisible Watermarked Video**: A binary watermark is embedded in the least significant bit (LSB) of the blue channel in selected frames.

## Features
- Adds **visible** watermarks with customizable text and opacity.
- Embeds **invisible** watermarks for potential use cases like copyright protection.
- Processes video files or searches for the first valid video file in a folder.
- Randomly selects additional frames for watermarking while ensuring critical frames (first, last) are always watermarked.
- Outputs videos in `.mp4` format.

## Prerequisites
Ensure you have Python installed along with the required libraries:
```bash
pip install opencv-python numpy
