# **Project & Onboarding Guide: Uncovering Urban Dynamics** 🚀

This document provides a complete guide to setting up the project.

---


### **1.1 Prerequisites**

Before you begin, please make sure you have the following software installed:
* **Git:** For version control.
* **Python 3:** The programming language we'll be using.

### **1.2 Project Setup**

Follow these steps precisely to create a consistent development environment.

#### **Step 1: Clone the Repository**
Open your terminal, navigate to where you want to store the project, and run the following command:
```bash
# Make sure to replace <repository_url> with the actual URL
git clone <repository_url>
cd sjsf-public-safety-mining
```

#### **Step 2: Download the Data**
1. Go to the [DataSF SFPD Incidents page](https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783).
2. Click **Export** and download the data as a CSV file.
3. Inside the project folder, create a new directory structure: `data/raw/`.
4. Move the downloaded file into that new folder and rename it to `sfpd_incidents.csv`.
5. The final path should be: `sjsf-public-safety-mining/data/raw/sfpd_incidents.csv`.

#### **Step 3: Create & Activate the Virtual Environment**
We use a virtual environment to keep our project's libraries isolated.

**Create the environment:**
```bash
python3 -m venv venv
```

**Activate the environment:**
* On macOS or Linux:
  ```bash
  source venv/bin/activate
  ```
* On Windows:
  ```bash
  .\venv\Scripts\activate
  ```

#### **Step 4: Install Dependencies**
Once the environment is activated, your terminal prompt will show `(venv)`. Now, install all the required libraries:
```bash
pip install -r requirements.txt
```

#### **Step 5: Create and Select the Jupyter Kernel**
This step ensures VS Code uses our dedicated project environment.

**Install ipykernel:**
```bash
pip install ipykernel
```

**Register the kernel:**
```bash
python -m ipykernel install --user --name=sjsf-crime-analysis --display-name="Python (SF Crime Analysis)"