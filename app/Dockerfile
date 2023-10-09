# Use an official Python runtime as an image
FROM python:3.8-slim-buster

# Sets the working directory for following COPY and CMD instructions
# Notice we haven’t created a directory by this name - this instruction
# creates a directory with this name if it doesn’t exist
WORKDIR /app

COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt

COPY . .

# Run app.py when the container launches
CMD ["python3", "app.py"]