# Computer Infrastructure Project: Data Analytics with Weather Data  

## Overview  
This repository contains the work for a project in the Computer Infrastructure module, which is part of the Higher Diploma in Computing in Data Analytics. The project focuses on using command-line tools, shell scripting, and Python (via Jupyter Notebook) to manage and process data, automate workflows, and analyze weather data. The repository also includes an automated process using GitHub Actions to ensure that weather data is updated daily and pushed to the repository.

## Automation with GitHub Actions  
- A GitHub Actions workflow has been implemented to automate the daily execution of the `weather.sh` script.  
- This workflow downloads the latest weather data, saves it in a timestamped file, and pushes the updates to this repository.

## Repository Contents  
The repository includes the following files and directories:
- **.github/workflows**: Directory containing GitHub Actions workflows for automating the script execution and pushing updates to the repository.
- **/data**: Directory containing subdirectories for storing timestamp data and weather data.
  - **/timestamps**: Contains the files `now.txt` and `formatted.txt` that store timestamp data.
  - **/weather**: Stores downloaded weather data files in JSON format, with timestamped filenames.
- **.gitignore**: A file that specifies which files and directories should be ignored by Git (e.g., virtual environments, temporary files).
- **README.md**: This file, containing an overview of the project and how to use it.
- **requirements.txt**: A file that lists the required Python packages for the project.
- **weather.ipynb**: A Jupyter Notebook summarizing the project, automating weather data collection, and analyzing it with pandas.
- **weather.sh**: A bash script that automates the download and timestamping of weather data.

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
  git clone <[repository-url](https://github.com/jakedaly97/computer-infrastructure-assessment)>  
  cd <computer-infrastructure-assessment>  
  ```  

#### 2. Using Anaconda  
- Ensure [Anaconda](https://anaconda.org/anaconda/python) is installed on your machine.  
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
- Ensure [VS Code](https://code.visualstudio.com/) and the Python extension are installed.  
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
## Requirements File  

The repository includes a `requirements.txt` file that lists the necessary Python packages for the project. To install the dependencies in this file, you can use **pip** after setting up your Python environment. Run the following command:

```bash
pip install -r requirements.txt
```

Alternatively, if you are using Anaconda, you can install the dependencies after creating and activating your environment with the following command:

```bash
conda activate weather_project
pip install -r requirements.txt
```

This will ensure that all required libraries (such as `pandas`, `requests`, and others) are installed for the project to function correctly.
## Acknowledgments  
- **Met Éireann**: For providing weather data.  
- **data.gov.ie**: For detailed dataset documentation.  
- **Higher Diploma in Computing in Data Analytics**: For the opportunity to work on this project.  

## Get Help

For assistance, users can refer to the comments within the project, providing insights into the written code. Additional clarification can be found in the Python documentation available at [Python Docs](https://docs.python.org/3/), or through numerous tutorials on Python, accessible on the W3Schools website at [W3Schools Python Tutorials](https://www.w3schools.com/python/default.asp). For further assistance, users can contact fellow project contributors.

## Contributions

Currently, Jake Daly is the sole contributor to this project.

## Author

Jake Daly is a part-time student enrolled in the Higher Diploma in Science in Computing in Data Analytics course at Atlantic Technological University.

For inquiries or further information, Jake can be contacted via:

Student Email: g00439324@atu.ie
Personal Email: jakedaly1997@hotmail.com
