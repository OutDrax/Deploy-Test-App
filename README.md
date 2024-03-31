# Project Sea Lanka
AI-Powered Prediction System for Identifying Optimal Fishing Zones and Species in the Coastal and Deep Waters of Sri Lanka. Utilizing environmental factors such as sea surface temperature and chlorophyll levels. The system will also incorporate past fish catch history data. The primary audience for this project includes fishermen and fish researchers, with the main objective being the enhancement of fish catch efficiency.

## **Prerequisites**

Before you begin, ensure you have the following installed:

- Node.js and npm (for the backend)
- Python 3.10 and pip (for the Flask microservice)
- Flutter (for the frontend app)

## **Cloning the Repository**

Start by cloning the repository to your local machine:

```bash
git clone https://github.com/yourusername/Project-Sea-Lanka.git
cd Project-Sea-Lanka
```

## **Setting Up the Environment for Python**

1. **Create a Virtual Environment**: After cloning the repository, you should navigate to the python project directory and create a new virtual environment. This can be done using:
    
    ```bash
    cd model_service
    python -m venv venv
    ```
    
    This command creates a new virtual environment named **`venv`** within the project directory.
    
2. **Activate the Virtual Environment**: Before installing any packages, you need to activate the virtual environment. The activation command varies depending on the operating system:
    - On Windows:
        
        ```
        .\venv\Scripts\activate
        ```
        
    - On macOS and Linux:
        
        ```bash
        source venv/bin/activate
        
        ```
        
3. **Install Dependencies**: With the virtual environment activated, you can install the project's dependencies using the **`requirements.txt`** file provided:
    
    ```bash
    pip install -r requirements.txt
    ```
    

## **Setting Up Node Environment**

1. **Navigate to the `node_backend` Directory**: Change into the **`node_backend`** directory from the root of the project:
    
    ```bash
    cd node_backend/
    ```
    
2. **Install Dependencies**: Run the following command to install the necessary npm packages:
    
    ```
    npm install
    ```
    
3. **Environment Variables**: Copy the **`.env.example`** file to a new file named **`.env`** and update the variables to match your local environment settings.
    
    ```bash
    cp .env.example .env
    ```
    

## Setting up ML model

Download the machine learning model from the provided link and place it in the **`model_service/model`** directory. If you happened to use a different model, make sure to edit the model name in `app.py` file. https://drive.google.com/file/d/1fXGqDmMSRz1KkR0DIYTLAFTlLMoFSRlT/view?usp=sharing

## **Running the Application**

1. **Manually Running Each Component**:
If you prefer to run each component manually, follow these steps:
    
    a. **Start the Express Backend Server**:
    
    ```bash
    cd node_backend
    npm start
    ```
    
    b. **Start the Flask Microservice**:
    
    ```bash
    cd model_service
    python app.py
    ```
    
    c. **Run the Flutter Frontend**:
    Navigate to the `Flutter` directory and run the app on your device or emulator.
    

## **Accessing the Application**

- The backend should be accessible at **`http://localhost:YOUR_BACKEND_PORT`**.
- The Flask microservice should be accessible at **`http://localhost:YOUR_FLASK_PORT`**.
- The Flutter app should be set up to communicate with these services based on the configuration you provided.
