# NDVI Estimation Pipeline

## Introduction
Traditional crop health analysis involved ground surveying that needs to be done at different phenotypic stages which is error prone and the data is unreliable. Most recently the focus has been shifted towards precision agriculture, that uses UAVs mounted with multispectral cameras to do surveying and the results are then used to generate a health report using vegetation indices such as NDVI. Most vegetation indices use multispectral imagery to generate results, for example NDVI uses mainly Red and NIR bands. This method is not cost effective and the multispectral sensor has a lower spatial resolution compared to an RGB camera. In our proposed methodology, we have estimated the NDVI values using RGB imagery that provides a more cost-effective method using deep learning.

## Dataset
We have collected our own custom dataset by performing several breeding experiments at the National Agriculture Research Center, Islamabad, Pakistan.

**Download Link: ** https://drive.google.com/file/d/1NrOjqKNzkoxhjgnTPbVzZLDL6_Qmdudq/view?usp=sharing

The dataset contains raw sensor data containing both RGB and NIR information. In order to isolate the bands execute,

```
python sensor_correction+GT_NDVI.py
```