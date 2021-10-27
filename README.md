# SIFT based Instance Search
## Introduction
This project aims to develop a program to detect objects with datasets(a random set of images). The first method is SIFT Feature Matching. SIFT is a feature detection algorithm to detect the image features. This project used the feature matching method to find out the similarity. The second method is SSIM who consider image luminance, contrast and structure to evaluate similarity. 

## How to use
1. Clone this project
2. Put your datasets and test images into folder Images and Queires respectivily
3. Run the main program `Object_Detection.ipynb` with [jupyterlab](https://jupyter.org/)

> Dataset Image Format: 0001.jpg, 0002.jpg, 0003.jpg, ... , 9999.jpg

> Test Image Format   : 01.jpg, 02.jpg, 03.jpg, ... , 99.jpg

### File Structure
```
.
├── Images                  # Datasets folder
│   ├── 0001.jpg
│   ├── 0002.jpg         
│   ├── ...         
├── Queries                 # Test files folder
│   ├── 01.jpg
│   ├── 02.jpg         
│   ├── ...      
└── Object_Detection.ipynb  # Main Program
```
## Result
### Summary
Dataset Size: 5000 images
|Item|SIFT|	SSIM|
|---|---|---|
|Mean average precision|	0.332950	|0.011360|
|Time|	2.5 hr	|20 mins |

### Details Comparison
![GitHub Logo](/sift_ssim_result.png)

## Short Review
1. SIFT is too slow for matching. It should combine with Bag of Word.
