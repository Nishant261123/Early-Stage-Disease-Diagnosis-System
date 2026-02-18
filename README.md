# Early-Stage-Disease-Diagnosis-System

An AI-powered web application for detecting nail diseases using Deep Learning (Transfer Learning with VGG16). The system supports both image upload and live webcam capture for real-time disease prediction.

🚀 Features  
✅ Detects 17 different nail diseases  
✅ Built using Transfer Learning (VGG16)  
✅ Upload image or capture via live webcam  
✅ Displays prediction with confidence score  
✅ Modern responsive UI (Flask + HTML + CSS + JS)  
✅ Drag-and-drop upload support  

🦠 Detected Diseases  
Darier's disease  
Muehrcke's lines  
Alopecia areata  
Beau's lines  
Bluish nail  
Clubbing  
Eczema  
Half and half nails (Lindsay's nails)  
Koilonychia  
Leukonychia  
Onycholysis  
Pale nail  
Red lunula  
Splinter hemorrhage  
Terry's nail  
White nail  
Yellow nails  

📂 Project Structure  

Nail-Disease-Prediction/
│
├── templates/
│   ├── index.html
│   ├── about.html
│   ├── nailhome.html
│   └── nailpred.html
│
├── static/
│   └── style.css
│
├── uploads/              # Auto-created temporary folder
├── main.py               # Flask backend
├── requirements.txt
├── .gitignore
└── README.md


⚠ Note:
Dataset and trained model file are NOT included in this repository due to GitHub size limitations.

🧠 Model Information  
Architecture: VGG16 (Transfer Learning)  
Input Size: 224 × 224  
Output: 17-class classification  
Framework: TensorFlow / Keras  

📥 Model Download  
The trained model file (vgg-16-nail-disease.h5) is not uploaded due to GitHub file size restrictions.  
Download it from:  
https://drive.google.com/drive/folders/1vQlPB_a31Ad4wLNQDnJLmK8DagXBcHeG?usp=sharing  

After downloading:
Place the file in the project root directory  
Ensure the filename matches:
model = load_model("vgg-16-nail-disease.h5")

📊 Dataset  
The dataset is not included in this repository due to its large size.  
Download it from:  
https://drive.google.com/drive/folders/1vQlPB_a31Ad4wLNQDnJLmK8DagXBcHeG?usp=sharing  

⚙ Installation  

Prerequisites:
Python 3.8+  
pip  

Step 1: Clone Repository  
git clone https://github.com/rohitt08-l/Early-Stage-Disease-Diagnosis-System.git  
cd nail-disease-detection  

Step 2: Install Dependencies  
pip install -r requirements.txt  

Step 3: Add Model File  

Place:
vgg-16-nail-disease.h5  
inside the root directory.

▶ Running the Application  
python main.py  

Open browser:
http://localhost:8080  

🖼 How to Use  

Go to NAIL → Predict  

Either:
Upload a nail image  
OR Capture live image via webcam  

Click Analyze Image  

View prediction + confidence score  

🛠 Technologies Used  

Backend:
Flask  
TensorFlow / Keras  
NumPy  
Pillow  

Frontend:
HTML5  
CSS3  
JavaScript  
WebRTC (Live Camera Capture)  
Font Awesome  

⚙ Configuration  

Change Port  

In main.py:
app.run(debug=True, port=8080)

Use Different Model  

Replace model file and update:
model = load_model("your-model-name.h5")

🚀 Future Enhancements  

Cloud deployment (Render / AWS / Railway)  
User authentication  
Store prediction history  
REST API for mobile integration  
Improved medical reporting system  
Grad-CAM visualization  

⚠ Disclaimer  

This application is developed for educational and research purposes only.  
It is not a substitute for professional medical advice, diagnosis, or treatment.  
Always consult a qualified healthcare professional.

👨‍💻 Author  
Nishant Mohite  
CSE Engineering Student