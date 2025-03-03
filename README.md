![Project Image](Picture_ReadMe/p1-completed-aws-udacity-Julieta_Rubis.webp)

AWS AI & ML Scholarship: Use a Pre-trained Image Classifier to Identify Dog Breeds

## Overview
This project is part of the AWS AI & ML Scholarship Program (Udacity). It utilizes pre-trained deep learning models (e.g., AlexNet, VGG, ResNet) to classify images of dogs into their respective breeds.

## Features
- Pre-trained Models: Implements AlexNet, VGG, and ResNet for classification.
- Dataset Handling: Uses a dataset of pet images for training and evaluation.
- Performance Metrics: Computes classification accuracy and error statistics.
- Command-line Interface (CLI): Provides options to run models with various parameters.
- AWS Integration: Can be deployed on AWS EC2 for cloud-based inference.

## Repository Structure
Use-a-Pre-trained-Image-Classifier-to-Identify-Dog-Breeds
README.md                 # Project Documentation (this file)
pet_images                # Dataset folder (input images)
uploaded_images           # Images processed for classification
__pycache__               # Cached Python files
dognames.txt              # List of dog breeds
imagenet1000_clsid_to_human.txt # ImageNet class-to-human mapping
alexnet_uploaded-images.txt   # AlexNet model results
resnet_uploaded-images.txt    # ResNet model results
run_models_batch.sh       # Shell script for batch execution
run_models_batch_uploaded.sh  # Shell script for uploaded images
Scripts (Core Functionality)
   - adjust_results4_isadog.py      # Adjusts classification results
   - calculates_results_stats.py    # Computes model performance stats
   - check_images.py                # Verifies image inputs
   - classify_images.py             # Core classifier script
   - get_input_args.py              # Handles command-line arguments
   - get_pet_labels.py              # Extracts labels from dataset
   - print_results.py               # Displays classification results
   - test_classifier.py             # Test script for model performance

## Installation & Setup
1.  Clone the Repository
   git clone https://github.com/yourusername/Use-a-Pre-trained-Image-Classifier-to-Identify-Dog-Breeds.git
   cd Use-a-Pre-trained-Image-Classifier-to-Identify-Dog-Breeds
2. Install Dependencies
   Ensure you have Python 3 and required libraries installed:
   pip install -r requirements.txt  # (Create if needed)
3. Run the Classifier
   To classify pet images using AlexNet:
   python check_images.py --dir pet_images --arch alexnet --dogfile dognames.txt
  For ResNet:
  python check_images.py --dir pet_images --arch resnet --dogfile dognames.txt

## Example Output
Model: AlexNet
Total Images: 1000
Correctly Classified: 923 (92.3%)
Incorrectly Classified: 77 (7.7%)

## Key Learnings
- Implemented transfer learning using pre-trained models.
- Used command-line arguments to improve usability.
- Computed model statistics for accuracy comparison.
- Explored AWS EC2 deployment for large-scale inference.

## Contributing
1. Fork the repository.
2. Create a new branch (feature-xyz).
3. Commit and push changes.
4. Open a Pull Request.

## License
This project is open-source under the MIT License.

⭐ Like this project? Give it a star on GitHub! ⭐
