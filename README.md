# ChatApp  

This repository contains the source code for **ChatApp**, a Django-based application. Follow the steps below to set up and run the project locally.  

---

## Prerequisites  
Ensure you have the following installed on your system:  
- Python 3.6 or later  
- pip (Python package manager)  

---

## Setup  

### Step 1: Clone the Repository  
```bash  
git clone <repository-url>  
cd ChatApp  
```  

### Step 2: Create a Virtual Environment  
To isolate dependencies, create a virtual environment:  
```bash  
python -m venv venv  
```  

### Step 3: Activate the Virtual Environment  

- On **Windows**:  
  ```bash  
  venv\Scripts\activate  
  ```  

- On **Mac/Linux**:  
  ```bash  
  source venv/bin/activate  
  ```  

### Step 4: Install Dependencies  
Install the required packages:  
```bash  
pip install -r requirements.txt  
```  

### Step 5: Install Additional Packages  
To enable WebSocket and ASGI capabilities:  
```bash  
python -m pip install -U channels  
python -m pip install -U daphne  
```  

### Step 6: Apply Database Migrations  
Prepare and apply database migrations:  
```bash  
python manage.py makemigrations  
python manage.py migrate  
```  

### Step 7: Create a Superuser  
Create an admin account for accessing the admin panel:  
```bash  
python manage.py createsuperuser  
```  

### Step 8: Run the Development Server  
Start the server:  
```bash
python manage.py runserver  
```  

---

## Accessing the Application  
Once the server is running, open your browser and visit:  
[http://127.0.0.1:8000](http://127.0.0.1:8000)  

You can access the admin panel at:  
[http://127.0.0.1:8000/admin](http://127.0.0.1:8000/admin)  

---
