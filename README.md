# AutoVerify-ALPR

### OCR-Based Automatic License Plate Recognition and Vehicle Verification System

---

## Project Overview

SmartPlate-AI is an end-to-end Computer Vision project designed to automatically detect vehicle license plates, extract registration numbers using Optical Character Recognition (OCR), and verify vehicle information through a custom vehicle database.

The project combines Image Processing, Computer Vision, OCR, and Database Management techniques to automate vehicle identification and retrieve ownership and penalty information in real time.

The primary objective is to assist traffic management systems, parking facilities, toll collection systems, and law enforcement agencies in identifying vehicles and validating their registration details automatically.

---

![image alt](https://github.com/SuyashMathur-bit/PlateDetection/blob/21c40761b34f9cabe3a6b404b3610c80bfff46a0/Screenshot%202026-03-22%20232814.png)

![image alt](https://github.com/SuyashMathur-bit/PlateDetection/blob/83b7848383758c67bbe3dfef0d8d3db2d7fe377b/Screenshot%202026-03-22%20233444.png)
## Dataset

### Vehicle Database

Source: Custom Generated Vehicle Registry Database

Records: 100+ Vehicle Records

Data Type: Structured Vehicle Registration Data

### Database Fields

* Registration Number
* Owner Name
* Vehicle Model
* Vehicle Status
* Fine/Penalty Amount

### Sample Record

Vehicle Number: DL3CAY9324

Owner Name: Priya Verma

Vehicle Model: Maruti Swift

Status: Penalty

Fine Amount: ₹1200

---

## Tools & Technologies

### Programming Language

* Python

### Libraries

* OpenCV
* NumPy
* Pytesseract OCR
* Regular Expressions (Regex)
* OS Module

### Computer Vision Techniques

* Haar Cascade Classifier
* License Plate Detection
* Image Preprocessing
* Grayscale Conversion
* Binary Thresholding
* OCR Character Extraction

### Database Management

* Text-Based Vehicle Registry Database
* Fast Dictionary-Based Record Lookup

---

## Project Workflow

### Image Acquisition

The system accepts a vehicle image as input.

Supported Inputs:

* Vehicle Photographs
* Parking Camera Images
* Traffic Monitoring Images
* Static Vehicle Images

---

### License Plate Detection

A Haar Cascade Classifier is used to locate the vehicle license plate.

Objectives:

* Detect the license plate region
* Generate a bounding box around the plate
* Extract the Region of Interest (ROI)

---

### Image Preprocessing

Before OCR extraction, the detected plate undergoes preprocessing.

Techniques Applied:

* Image Resizing
* Grayscale Conversion
* Noise Reduction
* Otsu Thresholding

Benefits:

* Improved OCR Accuracy
* Better Character Visibility
* Reduced Recognition Errors

---

### Optical Character Recognition (OCR)

Pytesseract OCR is used to extract text from the detected license plate.

OCR Configuration:

* Character Whitelisting
* Page Segmentation Optimization
* Text Cleaning using Regex

Example:

Detected Plate:

DL3CAY9324

The extracted text is cleaned and standardized before verification.

---

### Vehicle Verification System

After OCR extraction, the registration number is matched against the custom vehicle database.

Retrieved Information:

* Owner Name
* Vehicle Model
* Registration Status
* Fine Information

Example Output:

Vehicle Number: DL3CAY9324

Owner: Priya Verma

Vehicle: Maruti Swift

Status: Penalty

Fine Amount: ₹1200

---

## Database Architecture

The project uses a custom database containing more than 100 vehicle records.

Database Features:

* Registration Verification
* Vehicle Ownership Lookup
* Fine/Penalty Tracking
* Instant Record Retrieval

Lookup Complexity:

O(1) average lookup using Python Dictionary Mapping

---

## System Architecture

Vehicle Image

↓

License Plate Detection

(OpenCV Haar Cascade)

↓

Image Preprocessing

(Resize + Thresholding)

↓

OCR Extraction

(Pytesseract OCR)

↓

Text Cleaning

(Regex Processing)

↓

Database Verification

(100+ Vehicle Records)

↓

Vehicle Information Retrieval

---

## Key Features

* Automatic License Plate Detection
* OCR-Based Text Recognition
* Vehicle Information Verification
* Fine/Penalty Status Lookup
* Real-Time Plate Processing
* Custom Vehicle Database Integration
* End-to-End ALPR Pipeline
* High Accuracy on Clear Vehicle Images

---

## Visualizations

The project includes:

### Detection Results

* Vehicle Image Display
* Bounding Box Around License Plate

### OCR Processing

* Thresholded Plate Image
* Extracted Registration Number

### Verification Results

* Vehicle Owner Information
* Vehicle Status
* Fine/Penalty Details

---

## Performance Highlights

* Successfully detects vehicle license plates using OpenCV.
* Accurately extracts registration numbers using Tesseract OCR.
* Verifies records against a database containing 100+ vehicles.
* Provides real-time ownership and violation information.
* Automates manual vehicle verification processes.

---

## Key Insights

* Image preprocessing significantly improves OCR accuracy.
* Thresholding enhances character extraction quality.
* OCR and database integration enable automated vehicle verification.
* Dictionary-based lookup ensures fast record retrieval.

---

## Business Impact

This project can help:

### Traffic Management Authorities

* Identify traffic violators
* Verify vehicle ownership
* Track penalty records

### Smart Parking Systems

* Automated vehicle entry and exit
* Vehicle registration verification

### Toll Collection Systems

* Fast vehicle identification
* Automated record validation

### Security Agencies

* Vehicle monitoring
* Suspicious vehicle tracking

### Smart City Applications

* Automated traffic surveillance
* Intelligent transportation systems

---

## Future Improvements

* YOLOv8-Based License Plate Detection
* Real-Time Video Stream Processing
* SQLite/MySQL Database Integration
* FastAPI/Flask Deployment
* Cloud-Based Vehicle Registry
* Multi-Country License Plate Support
* Vehicle Blacklist Detection System
* Deep Learning OCR Models
* Mobile Application Integration

---

## Repository Structure

```text

SmartPlate-AI/
│
├── Plate.py
├── Plate_image
├── README.md
├── Output_Screenshots/
├── Screenchots
├──database.txt
```

---

## Learning Outcomes

Through this project, I gained practical experience in:

* Computer Vision
* OpenCV Image Processing
* Optical Character Recognition (OCR)
* Object Detection Techniques
* Vehicle Verification Systems
* Database Integration
* Real-Time Information Retrieval
* Automated Surveillance Applications



