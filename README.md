# virtual-keybord-using-hand-gesture
Virtual Keyboard using Hand Tracking
Overview
This project demonstrates a virtual keyboard controlled by hand gestures using OpenCV, MediaPipe, and Pynput. The system uses a webcam to detect hand movements and translates these gestures into keyboard inputs.

Features
Hand Tracking: Utilizes MediaPipe to track hand movements and finger positions.
Virtual Keyboard: Displays a virtual keyboard on the screen which can be controlled using hand gestures.
Keyboard Input: Simulates keyboard inputs based on hand gestures and selected virtual keys.
Requirements
Python 3.x
OpenCV
MediaPipe
Numpy
Pynput
Installation
Clone the Repository

bash
Copy code
git clone https://github.com/your-username/virtual-keyboard.git
cd virtual-keyboard
Create a Virtual Environment (Optional but Recommended)

bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
Install Required Packages

bash
Copy code
pip install opencv-python mediapipe numpy pynput
Usage
Run the Script

Execute the Python script to start the virtual keyboard application.

bash
Copy code
python virtual_keyboard.py
Controls

Select Keyboard Layout:
"APR" Key: Switches between two layouts ("up" and "down") when pressed.
Keyboard Actions:
"CL" Key: Clears the current text.
"SP" Key: Inserts a space.
"APR" Key: Toggles between different layouts.
Alphabet Keys: Type the corresponding character.
Exit the Application

Press the q key to exit the application.

Code Explanation
Hand Tracking: Uses MediaPipe to detect hand landmarks and specifically tracks the index finger for interacting with the virtual keyboard.
Virtual Keyboard: The keyboard is drawn on the screen with buttons for each key. The virtual keyboard layout can be toggled between different configurations.
Button Interaction: When the index finger is over a button for more than 3 seconds, the corresponding key action is performed. This includes typing characters and special actions like space and backspace.
Troubleshooting
Camera Not Detected: Ensure that your webcam is properly connected and accessible. Try using different USB ports or checking camera permissions.
Performance Issues: Make sure you are running the script on a capable machine and close other applications that might be using significant resources.
Contributing
Feel free to open issues or pull requests for improvements and bug fixes. Contributions are welcome!

License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgements
MediaPipe: MediaPipe Documentation
OpenCV: OpenCV Documentation
Pynput: Pynput Documentation
