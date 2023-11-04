# Referral Microsystem for Transendity

## Introduction
The Referral Microsystem is a Flask-based service dedicated to managing the referral system for Transendity, a cutting-edge online money service application. This microservice is designed for high flexibility, capable of operating as a standalone service or integrated within a broader ecosystem. It centralizes referral tracking, reward calculations, and facilitates seamless API endpoint integrations for expanded functionality.

## Features
- Robust user referral tracking
- Automated referral reward calculation and distribution
- Secure API endpoints for easy referral management
- Independent service functionality powered by Flask
- Smooth integration with main applications and chatbot interfaces
- Secure and scalable user authentication using OAuth standards

## Technology Stack
- **Framework**: Flask (Python) for backend API and serving front-end pages
- **Database**: PostgreSQL for reliable, transactional data storage
- **Front-end**: Jinja2 templates, HTML/CSS for intuitive web interfaces
- **Authentication**: OAuth protocol with [Specify Provider] for secure access control
- **Deployment**: AWS Elastic Beanstalk for scalable cloud deployment

## Getting Started

### Prerequisites
To get started with this project, you'll need to have Python and PostgreSQL installed on your system.

```bash
# Check Python version
python --version

# Install Python and pip if not installed
sudo apt install python3 python3-pip

# Install PostgreSQL
sudo apt update
sudo apt install postgresql postgresql-contrib

```

### Setup

```bash
# Clone the repository
git clone [Your Repository URL]

# Navigate to the project directory
cd referral-microsystem

# Install Python dependencies
pip install -r requirements.txt

# Create a .env file for environment variables
touch .env

```

### Running Locally

```
# Then edit the .env file to include DATABASE_URL, OAUTH_PROVIDER_DETAILS, and other necessary configurations.

# Run database migrations (make sure to set up your database and migrations first)
flask db upgrade

# Start the Flask server
flask run

```

### Deployment

```
# Install the EB CLI tools if not already done
pip install awsebcli

# Initialize Elastic Beanstalk application
eb init -p python-3.6 referral-microsystem --region [Your Preferred AWS Region]

# Create an Elastic Beanstalk environment and deploy the application
eb create referral-microsystem-env

# After successful deployment, open your application in the browser
eb open

```

## Contributions

Initial contribution for the Referral Microsystem project was provided by:

- Rajgursher Singh - *Project Initiator and Lead Developer*

We welcome contributions from the community. If you would like to contribute, please fork the repository and submit a pull request with your proposed changes.


## License

This project is licensed under the MIT License - see the LICENSE.md file for details.

