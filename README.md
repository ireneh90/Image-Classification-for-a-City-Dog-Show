# City Dog Show Image Classification

This project was completed as part of Udacity's **AI Programming with Python** coursework.

The goal is to use a pre-trained image classifier to identify whether submitted pet images contain dogs and, for dog images, determine the dog's breed. The project focuses on applying core Python programming skills rather than building the image classifier itself.


## Project Objectives

* Identify which images contain dogs and which do not.
* Correctly classify the breed of dog images.
* Compare the performance of three CNN architectures:

  * AlexNet
  * ResNet
  * VGG
* Compare classification accuracy with model runtime.


## Technologies

* Python
* PyTorch / Torchvision
* Pre-trained CNN models
* Command-line arguments with `argparse`


## Results

The models were tested on 40 pet images:

| Model   | Correct Dogs | Correct Non-Dogs | Correct Dog Breeds | Runtime |
| ------- | -----------: | ---------------: | -----------------: | ------: |
| AlexNet |         100% |             100% |              80.0% |      3s |
| ResNet  |         100% |              90% |              90.0% |      6s |
| VGG     |         100% |             100% |              93.3% |     20s |


## Conclusion

**VGG** provided the best overall classification performance. It correctly identified dogs and non-dogs with 100% accuracy and achieved the highest dog-breed classification accuracy at **93.3%**.

Although VGG required more runtime than AlexNet and ResNet, it produced the strongest overall results for the project objectives.


## Project Structure

Key files include:

* `check_images.py` — main program
* `get_input_args.py` — processes command-line arguments
* `get_pet_labels.py` — creates pet labels from image filenames
* `classify_images.py` — classifies images using the selected CNN model
* `adjust_results4_isadog.py` — determines whether labels represent dogs
* `calculates_results_stats.py` — calculates classification statistics
* `print_results.py` — prints final model results
* `run_models_batch.sh` — runs the program using all three CNN architectures


## Coursework Attribution

This project was completed as part of Udacity's AI Programming with Python Nanodegree coursework.

The project brief, starter files, project structure, image-classification framework, pre-trained CNN classifier, supporting datasets, and instructional/hint code were provided by Udacity as part of the course materials.

My work focused on completing the required Python programming tasks, including:

processing command-line arguments;
generating pet labels from image filenames;
using the provided classifier to classify images;
comparing classifier and pet-image labels;
determining whether labels represent dogs or non-dogs;
calculating classification statistics;
printing and interpreting model results; and
testing the completed program with additional uploaded images.

This repository is shared as a record of my coursework and learning. Credit for the original project design, starter code, course materials, and provided classification resources belongs to Udacity and the respective original authors.


## Image Attribution

The images used in the `uploaded_images` folder were sourced from the following publicly available webpages for educational purposes as part of this coursework:

*Cat_01.jpg — WebMD, Cats: https://www.webmd.com/pets/cats/default.htm
*Coffee_mug_01.jpg — Graham & Green, Blue Ceramic Mug: https://www.grahamandgreen.co.uk/blue-ceramic-mug
*Dog_01.jpg — Photowall, Golden Retriever Puppy: https://www.photowall.co.uk/golden-retriever-puppy-canvas-print
*Dog_02.jpg — A horizontally flipped version of `Dog_01.jpg`, created for the image-classification test as required by the project instructions.

These images were used solely for educational and non-commercial purposes. All rights to the original images remain with their respective rights holders.
