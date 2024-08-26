# Image to Sketch Converter

This Python script converts a given image into a pencil sketch using image processing techniques. It utilizes the `numpy`, `imageio`, `scipy`, and `cv2` (OpenCV) libraries to achieve this effect.

## Features
- Convert any image into a sketch using a few lines of Python code.
- The script uses grayscale conversion, image inversion, and Gaussian blurring to produce a realistic sketch effect.

## Requirements

To run this script, you need to install the following Python libraries:

- `numpy`
- `imageio`
- `scipy`
- `opencv-python`

You can install them using pip:

```bash
pip install numpy imageio scipy opencv-python
```

## How It Works

1. **Grayscale Conversion:** The script converts the image into grayscale using a weighted sum of the RGB channels.
2. **Image Inversion:** The grayscale image is inverted to create a negative effect.
3. **Gaussian Blurring:** The inverted image is blurred using a Gaussian filter to create a smooth transition between the light and dark areas.
4. **Dodge Blending:** The blurred image is combined with the original grayscale image using the Dodge blend technique, which results in a pencil sketch effect.

## Usage
Place the image you want to convert into the same directory as the script and rename it to `dog.jpg` or change the img variable in the script to the image's filename.

Run the script:
```bash
python image_to_sketch.py
```
The output will be saved as `sketchDog.png` in the same directory.

## Demo

![imgtosketch](https://github.com/user-attachments/assets/94e60ca9-96db-40e6-a0bf-2943d94c9486)

## What's Next?
Feel free to experiment with different images, tweak the Gaussian blur intensity, or even build a graphical user interface (GUI) to make the tool more user-friendly. The possibilities are endless—get creative and make this project your own!

