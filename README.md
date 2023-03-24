
# PROJECT NAME
 Team Charlie --- Auto-transcribe and open-data system in Fraktur.

## Vision
 Once the user upload a PDF file, the application will do following things:  
 1. Split the PDF by pages and save all pages as PNG.  
 2. Scan every page and transcribe the words from Fraktur to modern German.  
 3. Group the content and pages by session flexibly and generate many source files according to the sessions.  
 4. Upload those files onto site and make them accessible.
 5. The site allows user to search and highlight keywords to locate their target quickly.
 6. All things will be done automatically.  
  
## Requirements
 The system uses github actions to install packages.  
 If running the system locally. Packages below are reuqired:  
    pyyaml  
    mdutils  
    pillow  
    PyMuPDF  
    beautifulsoup4  
    pandas  
    webdriver-manager  
    selenium  
  
## Building the application
 There are three periods during our project with many steps:
 1. Django system  
   1.1 Find the OCR library  
   1.2 Use tesseract for transcribing (But not accurate)  
   1.3 Build Django work  
   1.4 Use Transkribus instead  
   1.5 Build many functions basing on Django (Creating, catagorying, searching, editing, deleting)  
 2. Jkan system  
   2.1 Build open data system basing on Jkan  
   2.2 Immigrate data gradually  
   2.3 Adjust the layout/categories/organization and many other configs  
   2.4 Add more functions according to requirements of customer  
 3. Automatic Jkan system  
   3.1 Use github actions  
   3.2 Write a python script to achieve all things automatically  

## Testing the build
How do I test the code to ensure the build is correct?
  
## Running the application
 The application will rerun it automatically powered by github actions.
  
## Team Members
 
 Chen Zhaoqi

 Deborah Duke  

 Gulnoza Khamidova

 Henry Lutterodt

 Isaac Laryea

 Tao Luo
