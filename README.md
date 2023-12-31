
# Audio Analysis and Visualization

This project is a Python script for analyzing audio files and visualizing the top musical notes detected in the audio. It utilizes the Fast Fourier Transform (FFT) to convert audio from the time domain to the frequency domain and identifies prominent musical notes based on their amplitudes.

## Features

- Audio analysis and note detection.
- Visualization of the top musical notes in the order they are played.
- Visualization of the audio waveform.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.x

## Usage

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/gtrtuugii/WAV-Notes-Converte.git
   ```

2. Change into the project directory:

   ```bash
   cd WAV-Notes-Converter
   ```

3. Run the script with your audio file:

   ```bash
   python3 fft_wav.py your_audio_file.wav
   ```

   Replace `your_audio_file.wav` with the path to your audio file.

4. The script will analyze the audio, detect musical notes, and display visualizations.

## Configuration

You can configure the script by modifying the following parameters in `main.py`:

- `FPS`: Frames per second for audio analysis.
- `FFT_WINDOW_SECONDS`: Window size in seconds for FFT analysis.
- To determine the number of top musical notes to detect during the analysis you can adjust the `num` parameter when calling the `find_top_notes` function based on your specific analysis requirements.

```python
# Example: Detect the top 5 notes
top_notes = find_top_notes(fft, num=5, xf=xf)
```

## Example

![example output matplotlib](https://github.com/gtrtuugii/WAV-Notes-Converter/blob/main/output/Figure_1.png?raw=true)

![example output matplotlib](https://github.com/gtrtuugii/WAV-Notes-Converter/blob/main/output/Figure_1b.png?raw=true)

## Acknowledgments

- [numpy](https://numpy.org/) - Numerical computing library for Python.
- [matplotlib](https://matplotlib.org/) - Plotting library for Python.
- [scipy](https://www.scipy.org/) - Scientific computing library for Python.



Feel free to contribute to this project by opening issues or pull requests.
