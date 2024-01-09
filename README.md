# ID Card Tampering Detection

## Overview
The ID Card Tampering Detection project aims to detect tampering in PAN cards using computer vision techniques. This project serves the purpose of verifying whether the PAN card provided by individuals, employees, or customers is authentic or altered.

## Project Description
The project involves comparing an original PAN card image with a user-uploaded PAN card image. It employs the following steps:

## Initial Setup and Image Processing
Utilizes Python libraries such as skimage, imutils, cv2, and PIL to perform image processing and analysis.
Downloads sample original and tampered PAN card images from external URLs for comparison.
Resizes and saves the images to a local directory in PNG format.
Converts the tampered image from RGBA to RGB and saves it as a JPEG file.

## Image Analysis
Calculates and displays image formats and sizes for both original and tampered images.
Computes the Structural Similarity Index (SSIM) between the grayscale versions of the images to determine their similarity.
Applies thresholding and contours to identify differences between the images, marking the areas of dissimilarity.

## Result and Summary
Displays the processed images, including the original, tampered, difference, and threshold images with contours.
Concludes with a summary indicating the SSIM (~31.3%) and infers that the user-provided image is potentially fake or tampered based on this comparison.

## Usage and Scope
The project can be implemented by various organizations for verifying different types of IDs like PAN, Aadhar, or Voter ID provided by their users or customers. It offers a simple means to identify potential tampering in the uploaded ID images.

## Note
The README provides an overview of the project and its functionality.
Users can replicate the steps outlined in the README to perform ID tampering checks.
