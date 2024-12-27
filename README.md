<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body style="font-family: Arial, sans-serif; line-height: 1.6;">
    <h1 style="text-align: center; color: #2c3e50;">Street View House Numbers (SVHN) Recognition with CNN</h1>
    <p>
        This project focuses on recognizing single-digit house numbers captured from real-world street images in the <strong>SVHN Dataset</strong>. 
        Unlike handwritten digits, this dataset contains images of numbers from urban environments, often captured in noisy, cluttered backgrounds.
    </p>
    <h2 style="color: #34495e;">Key Features</h2>
    <ul>
        <li><strong>Robust Handling of Real-World Challenges:</strong> The model addresses challenges like digit overlaps, blurriness, and noisy backgrounds.</li>
        <li><strong>Data Augmentation:</strong> Implements random rotations, affine transformations, and perspective distortions to increase training robustness.</li>
        <li><strong>Squeeze-and-Excitation Blocks (SEBlock):</strong> Enhances feature extraction by focusing on the most important channels in the convolution layers.</li>
        <li><strong>Class Weighting:</strong> Solves dataset imbalance by assigning higher weights to less frequent digits, ensuring fairer predictions.</li>
        <li><strong>Comprehensive Evaluation:</strong> Includes confusion matrix, classification report, and multi-class ROC curves for performance analysis.</li>
    </ul>
    <h2 style="color: #34495e;">Highlights</h2>
    <ul>
        <li><strong>Accuracy:</strong> Achieved <strong>92% accuracy</strong> on the SVHN test set after extensive optimization.</li>
        <li><strong>Misclassification Handling:</strong> Reduced confusion between similar digits like '9', '6', and '3' by refining the model and training process.</li>
        <li><strong>Robustness:</strong> Improved recognition of digits in low-quality images through enhanced data augmentation techniques.</li>
    </ul>
    <h2 style="color: #34495e;">How to Use</h2>
    <ol>
        <li><strong>Clone the repository:</strong>
            <pre><code>git clone https://github.com/Lidorpahima/Street_View_House_Numbers_Machine_Learning.git</code></pre>
        </li>
        <li><strong>Install dependencies:</strong>
            <pre><code>pip install -r requirements.txt</code></pre>
        </li>
        <li><strong>Train the model:</strong>
            <pre><code>python train.py</code></pre>
        </li>
        <li><strong>Evaluate the model:</strong>
            <pre><code>python evaluate.py</code></pre>
        </li>
    </ol>
    <h2 style="color: #34495e;">Visualization and Reports</h2>
    <ul>
        <li><strong>Confusion Matrix:</strong> Visualizes model predictions and highlights areas of misclassification.</li>
        <li><strong>Classification Report:</strong> Displays precision, recall, and F1-scores for each digit.</li>
        <li><strong>ROC Curve:</strong> Evaluates the model's ability to distinguish between classes with AUC scores close to 1.0 for all digits.</li>
    </ul>
    <h2 style="color: #34495e;">Future Work</h2>
    <p>
        Extend the model to recognize multi-digit house numbers and optimize its architecture for real-time applications, such as mobile or embedded systems.
    </p>
    <p style="text-align: center; color: #7f8c8d;">Feel free to explore, fork, and contribute to this project! 🚀</p>
</body>
</html>
