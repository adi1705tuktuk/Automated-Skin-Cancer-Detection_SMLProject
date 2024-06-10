# Automated Skin Cancer Detection

## Problem Statement
Skin cancer, particularly malignant melanoma, poses a significant health threat with increasing instances reported annually. Detecting skin lesions, a precursor to skin cancer, is challenging due to artifacts, low contrast, and visual similarities with benign features like moles or scars. The project aims to develop an automated and reliable system for skin cancer detection using machine learning and deep learning techniques.

## Dataset
The project utilizes the HAM10000 dataset, which consists of:

1. **HAM10000_metadata.csv**: A tabular dataset containing patient information, class IDs, sex, cancer location, and skin cancer disease type (dx).
2. **HAM10000_images**: A folder containing 10,015 image files representing different forms of skin cancer.

The dataset includes seven classes of skin cancer diseases: Benign Keratosis lesions (Bkl), Melanocytic nevi (Nv), Melanoma (Mel), Basal cell carcinoma (Bcc), Actinic keratoses (Akiec), Vascular lesions (Vasc), and Dermatofibra (Df).

## Methodology
1. **Data Preprocessing**: The image data was resized, grayscaled, and flattened for machine learning models. Feature selection and encoding were performed on the tabular data.
2. **Dimensionality Reduction**: Principal Component Analysis (PCA) and Autoencoders were used for dimensionality reduction.
3. **Handling Class Imbalance**: Oversampling (SMOTE) and undersampling techniques were employed to address class imbalance.
4. **Model Training and Evaluation**: Various machine learning models (Random Forest, AdaBoost, SVM, KNN, Logistic Regression, MLP, Naive Bayes, Decision Tree, Gradient Boosting, and XGBoost) were trained and evaluated using accuracy, precision, recall, and F1-score.
5. **Cross-Fold Validation**: K-fold cross-validation (with K=5) was performed to assess model performance.
6. **CNN Model**: A Convolutional Neural Network (CNN) model was developed and trained using only the image data.

## Results
The project provides a comprehensive analysis of different machine learning and deep learning models for skin cancer detection. The best-performing models, along with their evaluation metrics, are reported in the final report.

## Usage
To use this project, follow these steps:

1. Clone the repository: `git clone https://github.com/your-repo.git`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Download the HAM10000 dataset and place it in the appropriate directory.
4. Run the necessary scripts or notebooks to preprocess the data, train the models, and evaluate their performance.

## Acknowledgments
- The HAM10000 dataset was obtained from the Harvard Dataverse page.
- The project references various research papers and resources, which are cited in the final report.
