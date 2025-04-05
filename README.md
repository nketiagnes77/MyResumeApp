# Install dependencies
sudo apt update
sudo apt install python3 py3-pip

# Create project directory
mkdir devops-portfolio
cd devops-portfolio

# Create virtual environment
python3 -m venv venv
source venv/bin/activate

# Install requirements
pip install -r requirements.txt

# Run the app
export FLASK_APP=app.py
python -m flask run --host=0.0.0.0 --port=5000
