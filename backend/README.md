# Udaicity Trivia API App
  This is a Trivia questions app where you can add or delete questions and play the trivia.
## Getting Started

Pre-requisites and Local Development
To use this project you should have Python3, pip and node installed on your machine.

## Backend

1. Initialize and activate a virtualenv using:

   python -m virtualenv env
   source env/bin/activate

  - On windows use the following,
   source env/Scripts/activate

2. From the backend folder run

   pip install requirements.txt.

   All required packages are included in the requirements file.

3. To run the application run the following commands:
   - export FLASK_APP=flaskr
   - export FLASK_ENV=development
   - flask run
 
The application is running on http://127.0.0.1:5000/ by default.

## Frontend

From the frontend folder, run the following commands to start the client:
- npm install // only once to install dependencies
- npm start

By default, the frontend will run on localhost:3000.

### Error Handling:

Errors are returned as JSON objects in the following format:
  {
      "success": False,
      "error": 400,
      "message": "bad request"
  }
#### The API will return three error types when requests fail:

  400: Bad Request
  404: Resource Not Found
  422: Not Processable
  500: Internal server error