# Document-Deterioration-Classification-Using-Gabor-Filters-and-Ensemble-classifiers-and-LIME

## Abstract
In this era, when document preservation is of grave importance, the introduction of innovations to improve the quality of palm-leaf manuscripts becomes significant for the preservation of cultural heritage. These manuscripts deteriorate in various ways, which makes them difficult to preserve and read. The unique patterns of deterioration that can take place across each section of the same document are not easily captured by conventional methods. The current approach adopted uses chunks of palm-leaf manuscripts from documents and classifies them into deterioration types using multiple advanced machine-learning models. Multiple ensemble methods are used further to tune and increase the accuracy. After that, chunks are reassembled and tailored image enhancement is done based on the results. Wrapper forward feature selection to enhance the classification quality of the chunks and additionally Local Interpretable Model-agnostic Explanations (LIME) explainability is used to analyze features contributing to the different
classes. The proposed model outperforms traditional classification techniques by integrating chunk-wise classification with ensemble methods. It achieves a significant accuracy improvement, with Bagging Random Forest (RF) yielding the highest accuracy of 92%, compared to Support Vector Machines (SVM) and K-Nearest Neighbors (KNN) This demonstrates the model’s superior ability to handle the complexities of palm-leaf manuscript deterioration, providing a more accurate and reliable classification for document preservation.

---

This repository contains the implementation of a novel machine learning approach for classifying palm-leaf manuscripts based on deterioration levels. The project integrates feature extraction using Gabor filters, classification with ensemble methods, and interpretability with LIME to enhance the preservation and restoration of historical documents.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Results](#results)
- [Usage](#usage)
- [Future Work](#future-work)
- [Acknowledgments](#acknowledgments)

---

## Introduction
This project focuses on preserving cultural heritage by classifying palm-leaf manuscripts into good, medium, and bad categories. By employing advanced machine learning techniques, the project enhances the accuracy and reliability of document preservation methods.

## Features
- **Chunk-wise Image Segmentation**: Divides documents into manageable chunks for detailed analysis.
- **Feature Extraction with Gabor Filters**: Extracts textural features for classification.
- **Ensemble Classifiers**: Combines models like Random Forest, KNN, and SVM to improve accuracy.
- **Explainability with LIME**: Highlights features contributing to classifications for better interpretability.
- **Tailored Image Enhancement**: Applies different techniques based on document classes to boost restoration.

## Dataset
- **Source**: Includes 433 palm-leaf manuscript images.
- **Chunk Details**: Each image is divided into 256x256 pixel chunks, resulting in a total of 16,406 chunks.
- **Class Distribution**: 
  - Good: 4,624 chunks
  - Medium: 5,234 chunks
  - Bad: 6,548 chunks

## Methodology
![Alt Text](relative/path/to/image "Optional Tooltip")

The approach consists of the following steps:
1. Image Chunking
2. Feature Extraction using Gabor Filters
3. Feature Engineering and Forward Selection
4. Classification using Ensemble Methods
5. Aggregation of Chunk Predictions
6. Explainability using LIME


## Results
- **Best Model**: Bagging Random Forest with an accuracy of 92%.
- **Performance Metrics**: Precision, recall, and F1-scores were evaluated across models.
- **Comparison with Literature**: The proposed model outperforms existing methods by providing enhanced classification accuracy and better explainability.

## Usage
### Prerequisites
- Python 3.8+
- Libraries: `cv2`, `numpy`, `pandas`, `matplotlib`, `seaborn`, `scikit-learn`, `lime`, `mlxtend`

### Running the Model
1. Clone the repository.
2. Install the required libraries: `pip install -r requirements.txt`.
3. Place the dataset in the specified folder.
4. Execute the Jupyter Notebook to preprocess data, train models, and evaluate results.

## Future Work
- Integrating deep learning techniques such as CNNs or GANs to enhance restoration capabilities.
- Exploring image inpainting for reconstructing missing document sections.
- Expanding the model to classify other historical document types.

## Acknowledgments
Special thanks to Amrita Vishwa Vidyapeetham for infrastructure support and team members for their contributions.
