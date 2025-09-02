# Document_Structure_Analysis
📌 Overview
This project focuses on document structure analysis – the task of classifying and segmenting components of a document such as text, tables, figures, titles, and lists. It implements and compares three approaches:
•	Support Vector Machine (SVM) – Feature-based classification
•	Random Forest Classifier – Robust ensemble learning
•	Detectron2 (Mask R-CNN 50 FPN) – Deep learning for advanced layout detection
Trained on the PubLayNet dataset, the project demonstrates the trade-offs between computational efficiency (SVM, Random Forest) and high-accuracy deep learning (Detectron2).
________________________________________
✨ Features
•	Classifies document elements: Text, Tables, Figures, Titles, Lists
•	Uses both classical ML models and deep learning frameworks
•	Handles scanned images and PDFs of structured/unstructured documents
•	Achieves up to 95% accuracy on complex document layouts
•	Provides a comparative study of efficiency vs. precision
________________________________________
🛠️ Tech Stack
•	Programming Language: Python
•	ML Models: SVM, Random Forest
•	Deep Learning: Detectron2, Mask R-CNN, PyTorch
•	Dataset: PubLayNet (IBM Research)
•	Libraries: OpenCV, NumPy, Pandas, Scikit-learn, Matplotlib
________________________________________
🔬 Methodology
1. SVM-Based Approach
•	Extracted area, aspect ratio, rectangularity, contour, and texture features
•	Trained an SVM classifier for text, table, and figure detection
•	Achieved ~87% accuracy
2. Random Forest Classifier
•	Extracted features like area, aspect ratio, perimeter, compactness, and line detection
•	Ensemble of decision trees reduces overfitting
•	Achieved ~89% accuracy
3. Detectron2 (Mask R-CNN 50 FPN)
•	Used ResNet backbone with FPN for multi-scale feature extraction
•	Region Proposal Network (RPN) for bounding box suggestions
•	ROI Heads for classification + segmentation (Text, Table, Figure, Title, List)
•	Achieved 95% accuracy on text, with strong performance across all categories
