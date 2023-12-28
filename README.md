# Dog Breed Identification using Pre-trained Image Classifier

## Overview

This project is part of the AWS AI/ML Scholarship Program Nanodegree - AI Programming with Python. The goal of this project is to utilize pre-trained convolutional neural network (CNN) models, specifically ResNet, AlexNet, and VGG, to classify dog breeds from images. The project involves extracting pet image labels from filenames, classifying images using the CNN models, and analyzing the results to determine the accuracy of each model in identifying dog breeds.

## Project Structure

The project is organized into the following main components:

1. **check_images.py**: Python script for classifying pet images using pre-trained CNN models.
2. **get_input_args.py**: Python script for handling command line arguments.
3. **get_pet_labels.py**: Python script for extracting pet image labels from filenames.
4. **classify_images.py**: Python script for classifying pet images using the specified CNN model.
5. **adjust_results4_isadog.py**: Python script for adjusting the results dictionary to indicate whether the pet image label and classifier label are of a dog.
6. **calculates_results_stats.py**: Python script for calculating results statistics.
7. **print_results.py**: Python script for printing a summary of the results, including incorrectly classified dogs and breeds.
8. **print_functions_for_lab_checks.py**: Python script containing print functions for checking the lab.
9. **dognames.txt**: Text file containing names of all dogs from the classifier function and pet image files.

## How to Run

To run the project, follow these steps:

1. Open a terminal window.
2. Navigate to the project directory.
3. Run the command:

    ```bash
    python check_images.py --dir <directory_with_images> --arch <model> --dogfile dognames.txt
    ```

    Example:

    ```bash
    python check_images.py --dir pet_images/ --arch vgg --dogfile dognames.txt
    ```

## Results

The project generates a summary table with key statistics, including:

- Number of Images
- Number of Dog Images
- Number of Not-a-Dog Images
- % Correct Dogs
- % Correct Breed
- % Correct Not-a-Dog
- % Match

Additionally, the table includes counts for each model (ResNet, AlexNet, VGG) for metrics such as the number of images, the number of correct dogs, and the number of correct breeds.

Misclassified dogs and misclassified breeds are also printed if specified.

## Acknowledgments

- This project was completed as part of the AWS AI/ML Scholarship Program Nanodegree - AI Programming with Python.
- Special thanks to the mentors and contributors in the program.
