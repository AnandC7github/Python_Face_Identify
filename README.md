# Python Face Identifying Project

## Overview
This project implements a live streaming application using Flask and OpenCV for face and eye recognition. The application captures video frames from the user's camera, detects faces and eyes using Haar cascades, and displays the results in real-time through a web interface.

## Project Structure

- **Haarcascades Folder:**
  - Contains XML files for Haar cascades used in face and eye detection.
    - haarcascade_car.xml
    - haarcascade_eye.xml
    - haarcascade_frontalface_default.xml
    - haarcascade_fullbody.xml

- **Templates Folder:**
  - Contains HTML templates for the web interface.
    - index.html
    - result.html

- **app.py:**
  - Main Python script containing the Flask application and OpenCV video processing logic.
  - Establishes a video feed route for live streaming.
  - Utilizes Haar cascades for face and eye detection.
  - Renders HTML templates for the web interface.

- **requirements.txt:**
  - Lists the required Python packages for running the project.
    - flask
    - opencv-python

## Instructions

1. **Install Dependencies:**
   - Run the following command to install the required dependencies:
     ```
     pip install -r requirements.txt
     ```

2. **Run the Application:**
   - Execute the `app.py` script to start the Flask application:
     ```
     python app.py
     ```
   - Access the application by navigating to `http://127.0.0.1:5000/` in your web browser.

3. **Web Interface:**
   - The main page (`index.html`) displays live video streaming from your camera.
   - Detected faces and eyes are highlighted in real-time.

4. **Final Results:**
   - After stopping the application, you can view the final detection results on the `result.html` page.

## Notes

- Ensure that your camera is properly connected and accessible.
- The application uses Haar cascades for face and eye detection, which may have limitations in certain scenarios.
- Feel free to customize the Haar cascade XML files or explore more advanced face recognition techniques for improved accuracy.

## Credits

- This project is based on Flask and OpenCV.
- Flask: [https://flask.palletsprojects.com/](https://flask.palletsprojects.com/)
- OpenCV: [https://opencv.org/](https://opencv.org/)

## License

This project is licensed under the [MIT License](LICENSE).
