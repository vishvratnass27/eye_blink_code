# eye_blink_code

Creating a GitHub README for your code is a great idea! Here's a simple README that explains your code:

---

# Eye Blink Detection with Python

## Overview

This Python script detects eye blinks using OpenCV and performs actions when a blink threshold is reached. In this example, we use eye blinks to open specific websites, but you can customize it to perform any action you want.

## Dependencies

- Python 3.x
- OpenCV (`cv2`)
- PyAutoGUI

You can install PyAutoGUI using pip:

```
pip install pyautogui
```

## How it Works

1. The script captures video from your default camera (usually your webcam).
2. It detects faces in the video stream using a pre-trained Haar Cascade classifier.
3. For each detected face, it extracts the region of interest (ROI) where the eyes are likely to be.
4. Inside the ROI, it uses another Haar Cascade classifier to detect eyes.
5. The script checks for blinks by counting how many consecutive frames have no detected eyes.
6. When the blink threshold is reached for either the left or right eye, it simulates a "Win" key press to open the Start menu.
7. It types a URL into the Start menu search bar and presses Enter to open the specified webpage.

## Customization

- You can adjust the `blink_threshold` variable to control how many consecutive blinks are required to trigger the action.
- You can change the URLs in the `pyautogui.typewrite` lines to open different websites or perform other actions.

## Usage

1. Clone the repository.
2. Install the required dependencies.
3. Run the Python script.
4. Point your camera towards your face.
5. Blink your left or right eye (depending on your configuration) to trigger the action.

## Example

In the provided code, blinking the **left eye** opens a YouTube link, and blinking the **right eye** opens a Google search. Customize these URLs as needed.

## Author

- vishvratna shegaonkar

## License

This project is open-source and available under the [MIT License](LICENSE).

---
