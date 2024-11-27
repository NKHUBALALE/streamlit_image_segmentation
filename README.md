# Segmentation Model Web App

Welcome to the **Segmentation Model Web App**, a tool designed for satellite image analysis and segmentation. This application leverages deep learning to produce segmentation masks that can assist in various applications, such as optimizing telecommunications network design.


![WhatsApp Image 2024-11-26 at 07 29 59_88c516a2](https://github.com/user-attachments/assets/49c01994-eda3-4a76-b9b1-68bde4f3d398)


---

## Features

### **Home**
- Provides an introduction to the app's purpose.
- Step-by-step instructions for using the app.
- Option to download project documentation as a PDF.

### **Predictions**
- Upload a satellite image (JPG, PNG, JPEG) and generate a segmentation mask.
- Preview segmentation predictions with provided sample images.
- Side-by-side comparison of the original image and its segmentation mask.

### **Insights**
- Displays key performance metrics of the segmentation model (e.g., Accuracy and IoU).
- Interactive bar chart for visualizing metrics.

### **Images and Masks**
- View pairs of images and their corresponding segmentation masks.
- Select from predefined image-mask pairs for visualization.

### **Feedback**
- Submit feedback through a text input field.
- Feedback is saved for further analysis and improvements.

### **Meet the Team**
- Learn about the mission and team members behind this project.
- Profiles include photos, roles, emails, and LinkedIn profiles.

---

## How to Use

1. **Clone the Repository**
   ```bash
   git clone https://github.com/username/segmentation-model-app.git
   cd segmentation-model-app```
   
2.  **Install Requirements**
Ensure you have Python 3.8 or higher. Install the required libraries:
```pip install -r requirements.txt```


**Prepare the Segmentation Model**
- Place the trained segmentation model (`final_model_resunet_finetuned_lr_reduced_5.h5`) in the root directory.
- Ensure the model is compatible with the `dice_loss` function and uses `MeanIoU` as a metric.

4. **Run the App**

5. **Access the App**
Open your browser and go to `http://localhost:8501`.
```streamlit run app.py```

## File Structure

```segmentation-model-app/
├── app.py                  # Main Streamlit application
├── final_model_resunet_finetuned_lr_reduced_5.h5  # Pretrained model
├── requirements.txt        # Python dependencies
├── images/                 # Folder for images used in the app
│   ├── sample.png
│   ├── test_image1.jpg
│   └── test_image2.jpg
├── masks/                  # Folder for segmentation masks
├── user_feedback.txt       # File to store user feedback
└── README.md               # This README file
```

## Technologies Used

Python: Core programming language.

Streamlit: Interactive web application framework.

TensorFlow/Keras: Deep learning framework for segmentation.

OpenCV: Image processing library.

Pandas: Data manipulation and analysis.

Pillow: Image loading and processing.

---

## Future Updates

- **Height Prediction Capabilities**: Predict terrain elevation using satellite imagery.
- **Enhanced UI/UX**: Make the app more user-friendly and visually appealing.
- **Deployment**: Host the app on cloud platforms like AWS, GCP, or Streamlit Community Cloud.

---

## Team

Meet the passionate team behind this project:
- **Emmanuel Nkhubalale**: Data Science Intern | Team Lead  
- **Nolwazi Mndebele**: Data Science Intern | Project Manager  
- **Carroll Tshabane**, **Jan Motene**, **Zamancwabe Makhathini**, **Muwanwa Tshikovhi**, **Sibukiso Nhlengethwa**: Data Science Interns  

For more information, refer to the **Meet the Team** section in the app.

---

## Feedback

We welcome your thoughts and suggestions. Use the **Feedback** section in the app or contact us via the provided emails.

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.
