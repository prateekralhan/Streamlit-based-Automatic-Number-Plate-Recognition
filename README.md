# Streamlit based Automatic Number Plate Recognition 🚘🚙 [![Project Status: Active](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) [![](https://img.shields.io/badge/Prateek-Ralhan-brightgreen.svg?colorB=ff0000)](https://prateekralhan.github.io/)
A streamlit based implementation of Automatic Number Plate Recognition for cars and other vehicles using images or live camera feed.

----------------
#### This work is just an extended implementation of the [great work](https://github.com/mftnakrsu/Automatic_Number_Plate_Recognition_YOLO_OCR) done by [mftnakrsu](https://github.com/mftnakrsu) 
----------------

![Animation](https://user-images.githubusercontent.com/29462447/168387966-0b541b59-27e2-4e9b-a94a-102400ba210c.gif)

![live feed demo](https://user-images.githubusercontent.com/29462447/168388053-ad26adcb-595a-4a8e-8b12-4594cc9718b6.gif)

## Installation:
* Simply run the command **pip install -r requirements.txt** to install the necessary dependencies.

## Usage:
1. Clone this repository and install the dependencies as mentioned above.
2. Make a directory within this cloned repository with the name `.streamlit` *(Don't forget the dot !!)*.
3. Create a file `config.toml` in this directory *(Be aware of the file extension !!)*.
4. Copy-Paste the following contents in this file and save :
```
[theme]
primaryColor="#ffb5b5"
backgroundColor="#132743"
secondaryBackgroundColor="#407088"
textColor="#ffb5b5"
```

5. Navigate to the root directory of this repository and simply run the command: 
```
streamlit run app.py
```
Navigate to http://localhost:8501 in your web-browser.

![live feed](https://user-images.githubusercontent.com/29462447/168388224-bd63a5bf-4ef1-4643-93d2-f47c2bd71c18.png)
![pic](https://user-images.githubusercontent.com/29462447/168388233-ba5add0f-2c00-49ed-8f1a-decadaffecd9.png)


------------
## Results 
------------

| **Output Images**  | **Output Images**  |
|---------------------|-----------------------|
| ![pic1](downloads/output_Cars18.png)  | ![pic1](downloads/output_Cars23.png)  |
| ![pic2](downloads/output_Cars65.png)  | ![pic2](downloads/output_Cars78.png)  |
| ![pic3](downloads/output_Cars72.png)  | ![pic3](downloads/output_Cars9.png)  |

### Running the Dockerized App
1. Ensure you have Docker Installed and Setup in your OS (Windows/Mac/Linux). For detailed Instructions, please refer [this.](https://docs.docker.com/engine/install/)
2. Navigate to the folder where you have cloned this repository ( where the ***Dockerfile*** is present ).
3. Build the Docker Image (don't forget the dot!! :smile: ): 
```
docker build -f Dockerfile -t app:latest .
```
4. Run the docker:
```
docker run -p 8501:8501 app:latest
```

This will launch the dockerized app. Navigate to ***http://localhost:8501/*** in your browser to have a look at your application. You can check the status of your all available running dockers by:
```
docker ps
```
