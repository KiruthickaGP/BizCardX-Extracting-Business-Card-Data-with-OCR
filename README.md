**BizCardX: Extracting Business Card Data with Optical Character Recognition (OCR)**

**Introduction**
Business card data extraction using Optical Character Recognition (OCR) is a cutting-edge technology that streamlines the process of digitizing contact information from physical business cards. By harnessing the power of OCR, businesses can efficiently convert printed text on business cards into digital data, enabling easy integration into contact management systems and enhancing networking and customer relationship management efforts.

**Overview**
In this streamlit web app, you can upload an image of a business card and extract relevant information such as name, designation, company, contact details, location etc from it using easyOCR. You can view, modify or delete the extracted data in this app. This app would also allow users to save the extracted information into a database along with the uploaded business card image. The database would be able to store multiple entries, each with its own business card image and extracted information.

**1. Tools Installed**
Virtual Studio code
Jupyter notebook
Python 3.11.3 or higher
MySQL

**2. Required Libraries**

streamlit, easyocr, cv2, mysql-connector-python, pandas, re, matplotlib.
3. Import Libraries
Image handling libraries
import easyocr
import cv2
File handling libraries
import os
import re
SQL library
import mysql.connector as sql
Pandas, Matplotlib
import pandas as pd
import matplotlib.pyplot as plt
Dashboard libraries
import streamlit as st
from streamlit_option_menu import option_menu

**4. ETL and EDA Process**

a) Extracting the data
Extract the particular business card data by using easyocr.

b) Transforming the data
After the extraction process, the text data extracted is converted into a structured data in the form of dataframe.

c) Loading data
After the transformation process, the data in the form of dataframe is stored in the MySQL database.

d) Visualizing, Updating, deleting the data
The extracted data can be visualized using matlplotlib and in the form of dataframe.

The data can also be updated, modified and deleted from the database.

**User Guide**

Step 1. Home Tab
It provides a brief overview of the project and the tools required for the project.

Step 2. Upload and Extract Tab
In this tab, Browse a a business card file (image) using browse file button and upload the image in upload here section. The image will be processed, required data will be collected. The processed image will appear with collected data in the text format.
Upoad the data to MySQL by clicking upload to MySQL button.
The fetched data will appear in the form of data frame.

Step 3. Modify Tab
In this page, we can alter the data collected from a business card, uplaod the modified data to the SQL database and then we can view the modified data as well.
Similarly, we can delete the data from MySQL database.
