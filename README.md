# Computer Infrastructure Project: Data Analytics with Weather Data  

## Overview  
- This repository contains the work for a project in the **Computer Infrastructure** module, as part of the Higher Diploma in Computing in Data Analytics.  
- The project focuses on using command-line tools, shell scripting, and Python (via Jupyter Notebook) to manage data, automate workflows, and analyze weather data.  
- The repository also includes automation via GitHub Actions to ensure daily updates of weather data.  

## Repository Structure  
```
/data  
  /timestamps  
  /weather  
weather.ipynb  
weather.sh  
README.md  
```  

### Directory Details  
- **/data**: Root directory for project data.  
  - **/timestamps**: Contains timestamp-related files (`now.txt` and `formatted.txt`).  
  - **/weather**: Stores downloaded weather data in JSON format.  
- **weather.ipynb**: A Jupyter Notebook summarizing the project and analyzing weather data using pandas.  
- **weather.sh**: A bash script to automate weather data downloads with timestamped filenames.  

## Automation with GitHub Actions  
- A GitHub Actions workflow has been implemented to automate the daily execution of the `weather.sh` script.  
- This workflow downloads the latest weather data, saves it in a timestamped file, and pushes the updates to this repository.  

## Get Started  

### Prerequisites  
- **Linux** or a Linux-like environment (e.g., WSL, macOS terminal).  
- **Python 3.x** installed (ensure `pip` is available).  
- **Jupyter Notebook** installed (or available through Anaconda/Visual Studio Code).  
- **Git** and **GitHub CLI** installed.  

### Steps  

#### 1. Clone the Repository  
- Open a terminal and clone this repository to your local machine:  
  ```bash  
  git clone <repository-url>  
  cd <repository-name>  
  ```  

#### 2. Using Anaconda  
- Ensure Anaconda is installed on your machine.  
- Navigate to the repository directory in your terminal.  
- Create a new environment and install dependencies:  
  ```bash  
  conda create --name weather_project python=3.x -y  
  conda activate weather_project  
  pip install notebook pandas  
  ```  
- Start the Jupyter Notebook server:  
  ```bash  
  jupyter notebook  
  ```  
- Open `weather.ipynb` in your browser and run the notebook.  

#### 3. Using Visual Studio Code  
- Ensure VS Code and the Python extension are installed.  
- Open the repository directory in VS Code.  
- Install the recommended extensions if prompted (Python, Jupyter).  
- Open `weather.ipynb` and select your Python interpreter.  
- Run cells in the notebook directly within VS Code.  

#### 4. Using GitHub Codespaces  
- Navigate to the repository on GitHub.  
- Click the green **Code** button and select **Open with Codespaces**.  
- Wait for the Codespace environment to set up.  
- Once the Codespace is ready, open `weather.ipynb` in the editor.  
- The environment will already have Jupyter installed. Run the notebook directly in the browser.  

### Running the Bash Script  
#### 1. Make the script executable:  
  ```bash  
  chmod +x weather.sh  
  ```  
#### 2. Run the script:  
  ```bash  
  ./weather.sh  
  ```  

## Acknowledgments  
- **Met Éireann**: For providing weather data.  
- **data.gov.ie**: For detailed dataset documentation.  
- **Higher Diploma in Computing in Data Analytics**: For the opportunity to work on this project.  
