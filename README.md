# Brain Tumor Classification

## Overview
The Brain Tumor Classification project aims to develop a deep learning model that can accurately classify brain MRI scans into four categories: Glioma, Meningioma, Pituitary, and No Tumor. This application leverages advanced machine learning techniques, including transfer learning with the Xception model and custom CNN architectures, to provide reliable predictions that can assist healthcare professionals in diagnosing brain tumors.

## Features
- **Image Upload**: Users can upload brain MRI images in JPG, JPEG, or PNG formats for classification.
- **Model Selection**: Users can choose between a pre-trained Xception model and a custom CNN model for predictions.
- **Saliency Map Generation**: The application generates saliency maps that highlight the regions of the MRI that the model focuses on when making predictions, providing insights into the decision-making process of the model.
- **Prediction Results**: The application displays the predicted class along with the confidence level of the prediction.
- **Visualization**: A Plotly bar chart visualizes the probabilities for each class, enhancing the interpretability of the model's predictions.

## Installation
To set up the project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Brain-Tumor-Classification.git
   cd Brain-Tumor-Classification
   ```

2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up environment variables:
   Create a `.env` file in the root directory and add your Google API key:
   ```
   GOOGLE_API_KEY=your_api_key_here
   ```

## Usage
1. Run the application:
   ```bash
   streamlit run myApp.py
   ```

2. Open your web browser and navigate to `http://localhost:8501`.

3. Upload a brain MRI image and select the desired model for classification.

4. View the predicted class, confidence level, saliency map, and a detailed explanation of the model's prediction.

## Impact
The ability to accurately classify brain tumors using deep learning can significantly impact patient outcomes by:
- **Early Detection**: Facilitating early diagnosis of brain tumors, which is crucial for effective treatment.
- **Enhanced Decision-Making**: Providing healthcare professionals with additional insights through saliency maps, helping them understand the model's focus areas.
- **Resource Efficiency**: Reducing the workload on radiologists by automating the initial classification process, allowing them to focus on more complex cases.
- **Research Advancement**: Contributing to the growing field of medical AI, paving the way for further innovations in diagnostic tools.

## Contributing
Contributions are welcome! If you have suggestions for improvements or new features, please open an issue or submit a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- TensorFlow and Keras for providing the deep learning framework.
- Streamlit for enabling the creation of interactive web applications.
- Plotly for visualization tools.
- OpenCV for image processing capabilities.
- Google Generative AI for enhancing model explanations.