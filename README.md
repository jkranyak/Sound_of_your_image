# Advanced Image Color Palette to Music Converter

This project is an innovative web application that transforms images into unique musical compositions based on their color palettes. It separates the foreground and background of an image, analyzes the dominant colors, and generates a layered musical piece that represents these visual elements.

## Features

- Upload any image file
- Separate foreground and background elements
- Extract dominant colors from both foreground and background
- Convert colors to musical frequencies
- Generate distinct musical compositions for foreground and background
- Mix foreground and background audio with adjustable ratio
- Offer multiple musical scales and instruments
- Implement different rhythm patterns
- Visualize the dominant colors and generated audio spectrogram
- Play the generated music directly in the browser
- Download the generated music as a WAV file

## How It Works

1. **Image Processing**: The application uses the `rembg` library to separate the foreground from the background of the uploaded image.

2. **Color Analysis**: K-means clustering is used to identify the dominant colors in both the foreground and background.

3. **Color to Sound Conversion**: Each extracted color is mapped to a musical frequency. The RGB values of each color are used to calculate a corresponding frequency within a chosen musical scale.

4. **Music Generation**: Two musical pieces are generated - one for the foreground colors and one for the background colors. The composition uses the selected musical scale and implements complex rhythm patterns.

5. **Audio Mixing**: The foreground and background audio are mixed with an adjustable ratio.

6. **Visualization**: The dominant colors are displayed as color swatches, and a spectrogram of the generated music is created.

## Technologies Used

- Python
- Gradio (for the web interface)
- NumPy and Pandas (for data processing)
- Pillow (for image processing)
- scikit-learn (for K-means clustering)
- SciPy (for audio processing and signal filtering)
- Matplotlib (for spectrogram generation)
- rembg (for background removal)

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/image-to-music-converter.git
   ```

2. Install the required packages:
   ```
   pip install gradio numpy pandas Pillow scikit-learn scipy matplotlib rembg
   ```

3. Run the application:
   ```
   python app.py
   ```

## Usage

1. Open the application in your web browser.
2. Upload an image using the provided interface.
3. Adjust the parameters as desired:
   - Duration of the generated music
   - Tempo (BPM)
   - Musical scale
   - Foreground and background instruments
   - Rhythm pattern
   - Foreground/background mix ratio
   - Music complexity
4. Click the "Submit" button.
5. View the extracted color palettes and listen to the generated music.
6. Download the audio file if desired.

## Customization

You can customize various aspects of the music generation process by modifying the corresponding functions in the code:

- `INSTRUMENTS`: Add or modify instrument sound generation functions.
- `SCALES`: Define additional musical scales.
- `RHYTHM_PATTERNS`: Create new rhythm patterns.
- `color_to_pitch`: Adjust how colors are mapped to musical pitches.
- `create_advanced_audio`: Modify the core audio generation algorithm.

## Contributing

Contributions to this project are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
