🎨 Virtual Air Painting with Hand Gesture Recognition
This project implements a virtual air painting system using OpenCV, Mediapipe, and a Random Forest model for hand gesture recognition. The system allows users to draw in the air using hand gestures, with the ability to change colors and erase strokes.

🚀 Features
✅ Hand Gesture Recognition:

Uses Mediapipe to track hand landmarks

Uses a Random Forest model to classify hand gestures:

Open Palm → Stops writing

Writing Hand → Allows drawing

✅ Painting Features:

Draw using your index finger

Change colors dynamically

Erase or clear the canvas

Real-time visual feedback on the screen

✅ Optimized for Performance:

Efficient deque-based stroke storage

Fixed IndexError for seamless drawing

Smooth animations & real-time processing

🛠 Tech Stack
Python

OpenCV (for real-time video processing)

Mediapipe (for hand tracking)

Scikit-learn (for Random Forest classification)

📂 Folder Structure
bash
Copy
Edit
📦 Virtual-Air-Painting
 ┣ 📜 main.py           # Main application script
 ┣ 📜 hand_model.pkl    # Trained Random Forest model
 ┣ 📜 README.md         # Project documentation
 ┣ 📜 requirements.txt  # Dependencies list
🔧 Setup & Installation
1️⃣ Clone the Repository

bash
Copy
Edit
git clone https://github.com/your-username/Virtual-Air-Painting.git
cd Virtual-Air-Painting
2️⃣ Install Dependencies

bash
Copy
Edit
pip install -r requirements.txt
3️⃣ Run the Application

bash
Copy
Edit
python main.py
🖥️ Usage Instructions
1️⃣ Start the program and position your hand in front of the camera.
2️⃣ Select a color by pointing your index finger to the color buttons at the top.
3️⃣ Draw in the air by moving your index finger while the model detects a "Writing Hand."
4️⃣ Stop drawing by opening your palm.
5️⃣ Clear the screen by selecting the "CLEAR" button.

Press 'q' to exit the program.

📊 Model Training
The hand gesture recognition model was trained using Mediapipe for feature extraction and Random Forest for classification.

Preprocessing Pipeline
Capture Hand Landmarks using Mediapipe.

Extract Features (x, y coordinates of key landmarks).

Label Data:

"Open Palm" → 0

"Writing Hand" → 1

Train Random Forest model for classification.

Save the model as hand_model.pkl.

📝 TODOs & Future Enhancements
 Improve Model Accuracy with more training data

 Support Multiple Gestures for additional features

 Enhance UI with better button design

 Save Drawings as image files

👨‍💻 Contributors
👤 Your Name
📧 your-email@example.com

💡 Feel free to contribute and improve the project!

🏆 Acknowledgments
Mediapipe for hand tracking

OpenCV for real-time video processing

Scikit-learn for model training

📜 License
This project is licensed under the MIT License.