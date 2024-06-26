Change Detection with Modified CNNs on OSCD Dataset
Overview
This repository contains code and resources for performing change detection using multiple modified Convolutional Neural Networks (CNNs) on the Onera Satellite Change Detection (OSCD) dataset. Change detection is a critical task in remote sensing, involving the identification of significant changes between satellite images taken at different times.

Features
Implementation of several CNN architectures for change detection.
Modifications to standard CNNs to enhance performance on change detection tasks.
Preprocessing and augmentation techniques tailored for the OSCD dataset.
Evaluation metrics and visualization tools for assessing model performance.
Dataset
The Onera Satellite Change Detection (OSCD) dataset is used in this project. It consists of pairs of satellite images acquired at different times along with change masks indicating areas of significant change.

Download the dataset: OSCD Dataset
Structure:
bash
Code kopieren
OSCD/
├── train/
│   ├── images/
│   ├── labels/
├── test/
│   ├── images/
│   ├── labels/
Installation
Clone the repository:

bash
Code kopieren
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
Create a virtual environment and install dependencies:

bash
Code kopieren
python -m venv venv
source venv/bin/activate   # On Windows use `venv\Scripts\activate`
pip install -r requirements.txt
Usage
Data Preprocessing
Before training the models, preprocess the dataset using the provided script:

bash
Code kopieren
python preprocess.py --data_path ./OSCD
Training
Train the CNN models using the training script:

bash
Code kopieren
python train.py --config configs/model_config.yaml
Evaluation
Evaluate the trained models on the test set:

bash
Code kopieren
python evaluate.py --model_path ./checkpoints/model.pth --data_path ./OSCD/test
Visualization
Visualize the change detection results using the visualization script:

bash
Code kopieren
python visualize.py --model_path ./checkpoints/model.pth --data_path ./OSCD/test --output_path ./results
Models
The repository includes implementations of several modified CNN architectures:

Modified U-Net
ResNet-based CNN
VGG-based CNN
Custom CNN with attention mechanisms
Each model can be configured and trained using the corresponding configuration files located in the configs directory.

Results
Performance of the models is evaluated using metrics such as:

Precision
Recall
F1-Score
Intersection over Union (IoU)
Results and model checkpoints are saved in the results and checkpoints directories, respectively.

Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgements
The OSCD dataset: OSCD Dataset
