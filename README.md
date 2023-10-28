# Pet-Adoption-Prediction

Introduction

This project aims to predict the speed at which a pet gets adopted based on the pet's listing on the leading animal welfare platform website in Malaysia. The goal is to develop algorithms that can assess the adoptability of pets, potentially guiding shelters and rescuers to create more appealing pet profiles, thereby reducing animal suffering and euthanization rates.

Problem Statement

Millions of stray animals suffer on the streets or face euthanization in shelters globally. Finding homes for these animals is crucial to saving lives and creating happy families. Adoption rates are strongly correlated with the metadata associated with pets' online profiles, including text descriptions, photo characteristics, and supplementary image analysis.

Dataset Description

The dataset comprises tabular, text, and image data:

Tabular data includes information such as PetID, AdoptionSpeed, Type, Name, Age, Breed, Color, Gender, Size, Vaccination status, Health condition, and more.

Text data provides the description of each pet's profile, primarily in English, with some entries in Malay or Chinese.

Image data contains photos named in the format of PetID-ImageNumber.jpg, with associated JSON files from Google's Vision API providing image analysis like Face Annotation, Label Annotation, Text Annotation, and Image Properties.

File Descriptions

train.csv: Tabular and text data for the training set.

test.csv: Tabular and text data for the test set.

breed_labels.csv: Contains Type and BreedName for each BreedID (1 for dog, 2 for cat).

color_labels.csv: Contains ColorName for each ColorID.

state_labels.csv: Contains StateName for each StateID.

Prediction Task

predict the Adoption Speed of pets, categorized as follows:

0: Same-day adoption

1: Adoption between 1 and 7 days

2: Adoption between 8 and 30 days

3: Adoption between 31 and 90 days

4: No adoption after 100 days (there are no pets in the dataset that waited between 90 and 100 days)

Image Metadata

The supplementary image analysis includes Face Annotation, Label Annotation, Text Annotation, and Image Properties extracted using Google's Vision API. Images are named as PetID-ImageNumber.jpg and corresponding JSON files.
