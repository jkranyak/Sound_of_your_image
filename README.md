# Advanced Image Color Palette to Music Converter

This project is an interactive web application that converts the dominant colors of an uploaded image into a unique musical composition, separating foreground and background elements.

## Features

- Upload any image file
- Separate foreground and background elements of the image
- Extract dominant colors from both foreground and background using K-means clustering
- Convert colors to musical frequencies
- Generate distinct musical compositions for foreground and background
- Mix foreground and background audio for a layered musical experience
- Visualize the dominant colors for both foreground and background
- Play the generated music directly in the browser
- Adjust duration and tempo of the generated music

## How it Works

1. **Image Separation**: The application uses the `rembg` library to separate the foreground (e.g., people, objects) from the background of the uploaded image.

2. **Color Extraction**: K-means clustering is used to identify the 8 most dominant colors in both the foreground and background.

3. **Color to Sound Conversion**: Each extracted color is mapped to a musical frequency. The RGB values of each color are used to calculate a corresponding frequency.

4. **Music Generation**: Two short musical pieces are generated - one for the foreground colors and one for the background colors. The composition uses a pentatonic scale for better harmony and implements a basic rhythmic structure.

5. **Audio Mixing**: The foreground and background audio are mixed, with the foreground being more prominent.

6. **Visualization**: The dominant colors for both foreground and background are displayed as color swatches.

7. **Playback**: The generated music can be played directly in the browser using an audio player.

## Technologies Used

- Python
- Gradio (for the web interface)
- NumPy and Pandas (for data processing)
- Pillow (for image processing)
- scikit-learn (for K-means clustering)
- SciPy (for audio processing)
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
   python app.py
   ```

## Usage

1. Open the application in your web browser.
2. Upload an image using the provided interface.
3. Adjust the duration and tempo sliders if desired.
4. Click the "Submit" button.
5. View the extracted color palettes for foreground and background.
6. Listen to the generated music, which combines elements from both foreground and background colors.

## Future Improvements

- Implement more advanced music generation algorithms
- Play the background tones seperately from the foreground rounding out the music
- Add options for different musical scales and instruments
- Improve the color-to-frequency mapping for more pleasing sounds
- Add the ability to download the generated music as an audio file
- Enhance the background removal algorithm for more accurate separation

## Contributing

Contributions to this project are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
