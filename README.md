# Object Classification System

A production-ready deep learning pipeline designed for scalable and reproducible object classification. This project integrates industry-standard MLOps practices, including automated data orchestration, versioning with DVC, and containerization with Docker, all served through a high-performance FastAPI interface.

# 🚀 Key Features
 1. **Modular Pipeline Architecture**: Separated components for Data Ingestion, Validation, Transformation, and Model Training to ensure clean, maintainable code.

 2. **Version Control with DVC**:  Integration: Full data and model versioning, ensuring reproducibility by tracking datasets and weights outside of Git.

 3. **Google Drive Dataset Sync**: Automated fetching of large-scale datasets directly from Google Drive storage.

 4. **FastAPI Web Interface**: A sleek, high-performance API for real-time image classification and model interaction.

 5. **Dockerized Environment**: Fully containerized setup to eliminate "works on my machine" issues and simplify deployment.

 6. **Comprehensive Validation**: Automated data validation checks to ensure schema consistency before the training phase begins.


 # 🛠️ Installation Instructions

Follow these steps to set up the project locally:

1. Clone the Repository

Bash

    git clone https://github.com/harshkumar8a/Object-Classification.git

    cd Object-Classification

2. Create a Virtual Environment

Bash

    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate

3. Install Dependencies

Bash

    pip install -r requirements.txt

4. Data Setup (DVC)

Bash

    dvc init

Ensure you have access to the data storage, then pull the latest data:

Bash

    dvc pull


# 💻 Usage Examples

**Running the Pipeline**

You can trigger the entire MLOps pipeline (Ingestion to Training) by running:

Bash

    python main.py

**Starting the FastAPI Server**

Launch the web interface locally to perform inferences:

Bash

    uvicorn app:app --reload
Once started, navigate to http://127.0.0.1:8000/docs to access the interactive Swagger UI and upload images for classification.

**Containerization**

Using Docker To run the entire application within a container:

Bash

    docker build -t object-classifier .
    docker run -p 8080:8080 object-classifier



# Contact Me

**Email**: harshkumar811h@gmail.com

**LinkedIn**: [Link](https://www.linkedin.com/in/harshkumar-8h/)
