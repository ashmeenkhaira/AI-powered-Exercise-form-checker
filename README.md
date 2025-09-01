# AI-powered-Exercise-form-checker
1. Project Overview

This project uses your webcam, OpenCV, and MediaPipe Pose to analyze and provide real-time feedback on your form while performing dumbbell lateral raises.

The system:

Tracks arm movement and posture

Counts repetitions automatically

Provides form correction feedback (arm height, elbow straightness, shoulder relaxation, balance)

Displays milestone messages when you hit certain rep counts

👉 Perfect for fitness enthusiasts, trainers, or anyone working out at home who wants instant feedback to improve technique.

2. Demo Video

Check out the project in action:
Demo Video

3. Tech Stack

Python 3.x

OpenCV – Webcam input and video frame display

MediaPipe Pose – Real-time human pose estimation

NumPy – Angle calculations and numeric operations

4. Setup Instructions
1. Clone the repository
git clone https://github.com/your-username/dumbbell-lateral-raise-tracker.git
cd dumbbell-lateral-raise-tracker

2. Install dependencies
pip install opencv-python mediapipe numpy

3. Run the project
python lateral_raise_checker.py

5. Workflow & Usage

The script starts video capture from your webcam.

MediaPipe Pose detects key body landmarks in each frame.

The program calculates:

Shoulder-to-arm angles (to track lateral raises)

Elbow straightness

Neck/shoulder posture (to detect shrugging)

Balance between left and right arms

A rep counter increments only when both arms complete a raise together.

Milestone messages (e.g., “Good job! 10 reps!”) appear at specific counts.

Form feedback is shown directly on the live video:

"Raise left arm higher"

"Straighten right elbow"

"Relax shoulders down"

"Balance arm heights"

The overlay displays:

Rep count

Current stage (up or down)

Form feedback

Press q to exit.

6. Features ✨

✅ Real-time posture and form detection

✅ Rep counting with milestone tracking

✅ Smart form feedback (arm height, elbows, shoulders, balance)

✅ Minimal, clear UI overlay on the webcam feed

✅ Works offline with just a webcam
