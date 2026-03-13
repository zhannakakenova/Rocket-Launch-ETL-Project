# Rocket-Launch-ETL-Project

This project demonstrates a simple **ETL (Extract, Transform, Load) pipeline** implemented in Python.
The goal of this project is to collect rocket launch data from an external API, process the data, store it locally, and visualize the results.

---

# Project Steps

## 1. Extract

Rocket launch data was collected from the external API:

```
https://ll.thespacedevs.com/2.0.0/launch/upcoming
```

The API was accessed using the **requests** library, and the response was saved locally as a JSON file.

---

## 2. Transform

The JSON data was processed and converted into a **pandas DataFrame** to explore and analyze the structure of the dataset.

Important information extracted from the dataset includes:

* Launch name
* Launch date
* Rocket information
* Launch location
* Image URL

This step prepares the raw API data for further processing.

---

## 3. Load

The collected data and downloaded images were stored locally.

Project structure:

```
data/
    launches.json

images/
    img_0.jpg
    img_1.jpg
    ...
```

The JSON file stores the raw API response, while the images folder contains downloaded rocket launch images.

---

## 4. Visualization

Downloaded images were loaded from the local folder and visualized using **matplotlib** and **PIL**.

This step displays rocket launch images in a grid format.

---

## 5. Additional Task

An additional ETL example was implemented using the **Titanic dataset**.

The dataset was loaded from a CSV URL and processed using **pandas** for basic data exploration.

---

# Technologies Used

* Python
* requests
* pandas
* json
* os
* matplotlib
* PIL (Python Imaging Library)
