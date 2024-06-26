# Advanced Image Color Palette to Music Converter

This project is a sophisticated web application that transforms the dominant colors of an uploaded image into a unique and complex musical composition. It separates foreground and background elements, creating a layered musical experience based on the color palette of the image.

## Features

- Upload any image file
- Separate foreground and background elements of the image
- Extract dominant colors from both foreground and background using K-means clustering
- Convert colors to musical frequencies using an improved HSL-based algorithm
- Generate distinct, complex musical compositions for foreground and background
- Offer multiple musical scales (pentatonic, major, minor)
- Provide various instrument sounds (sine, square, sawtooth waves)
- Implement different rhythm patterns for added musical complexity
- Mix foreground and background audio for a layered musical experience
- Visualize the dominant colors for both foreground and background
- Play the generated music directly in the browser
- Download the generated music as a WAV file
- Adjust duration, tempo, scale, instrument, and rhythm pattern of the generated music

## How it Works

1. **Image Separation**: The application uses the `rembg` library to separate the foreground from the background of the uploaded image.

2. **Color Extraction**: K-means clustering identifies the 8 most dominant colors in both the foreground and background.

3. **Color to Sound Conversion**: Each extracted color is mapped to a musical frequency using an improved algorithm based on the HSL color space.

4. **Music Generation**: 
   - Two musical pieces are generated - one for the foreground colors and one for the background colors.
   - The composition uses the selected musical scale and implements complex rhythm patterns.
   - Chords and arpeggios are generated based on the color-derived frequencies.
   - The background music is processed with a low-pass filter for a more ambient sound.

5. **Audio Mixing**: The foreground and background audio are mixed, with the foreground being more prominent.

6. **Visualization**: The dominant colors for both foreground and background are displayed as color swatches.

7. **Playback and Download**: The generated music can be played directly in the browser and downloaded as a WAV file.

## Technologies Used

- Python
- Gradio (for the web interface)
- NumPy and Pandas (for data processing)
- Pillow (for image processing)
- scikit-learn (for K-means clustering)
- SciPy (for audio processing and signal filtering)
- rembg (for background removal)

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/advanced-image-to-music-converter.git
   ```

2. Install the required packages:
   ```
   pip install gradio numpy pandas Pillow scikit-learn scipy rembg
   ```

3. Run the application:
   ```
   python advanced_image_to_music.py
   ```

## Usage

1. Open the application in your web browser.
2. Upload an image using the provided interface.
3. Adjust the following parameters as desired:
   - Duration (5-30 seconds)
   - Tempo (60-180 BPM)
   - Musical Scale (pentatonic, major, minor)
   - Instrument (sine, square, sawtooth)
   - Rhythm Pattern (simple, syncopated, waltz, complex)
4. Click the "Submit" button.
5. View the extracted color palettes for foreground and background.
6. Listen to the generated music, which combines elements from both foreground and background colors.
7. Download the generated music as a WAV file if desired.

## Future Improvements

- Implement more advanced music generation algorithms (e.g., neural network-based)
- Add more instrument sounds and effects
- Enhance the background removal algorithm for more accurate separation
- Optimize performance for larger images or longer durations
- Implement user accounts to save and share creations

## Contributing

Contributions to this project are welcome! Please feel free to submit a Pull Request or open an Issue for discussion.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
