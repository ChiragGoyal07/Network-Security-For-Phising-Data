### Network Security Projects For Phising Data

This project aims to detect and mitigate phishing attacks using machine learning techniques. The solution leverages preprocessing, training, and deploying ML models to secure networks against phishing threats.

## Getting Started

Follow these instructions to set up the project on your local machine for development and testing purposes.

### Prerequisites

Ensure you have the following software and libraries installed:

- Python 3.8 or above
- pip
- Docker

Install the necessary Python dependencies by running:

```bash
pip install -r requirements.txt


### Installing

1. Clone the repository to your local machine:

   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the application using Docker (if applicable):

   ```bash
   docker build -t network-security .
   docker run -p 5000:5000 network-security
   ```

## Running the tests

### Break down into end-to-end tests

Run the test files to validate functionality. For example, you can test the MongoDB integration by running:

```bash
python test_mongodb.py
```

Ensure all tests pass to confirm the system works as expected.

## Deployment

To deploy the project on a live system, ensure the required environment is set up with the dependencies installed. Use Docker for easier deployment:

```bash
docker build -t network-security .
docker run -d -p 5000:5000 network-security
```

## Built With

- [Python](https://www.python.org/) - Programming language
- [MongoDB](https://www.mongodb.com/) - Database used
- [Flask](https://flask.palletsprojects.com/) - Web framework

## Versioning

This project follows [SemVer](http://semver.org/) for versioning. Refer to the tags in the repository for details.
```


Setup github secrets:
AWS_ACCESS_KEY_ID=

AWS_SECRET_ACCESS_KEY=

AWS_REGION = us-east-1

AWS_ECR_LOGIN_URI = 788614365622.dkr.ecr.us-east-1.amazonaws.com/networkssecurity
ECR_REPOSITORY_NAME = networkssecurity


Docker Setup In EC2 commands to be Executed
#optinal

sudo apt-get update -y

sudo apt-get upgrade

#required

curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker
