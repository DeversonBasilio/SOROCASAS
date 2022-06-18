FROM python:latest

# Setup all python related enviroment
ENV PYTHONDONTRWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# Set the working directory
WORKDIR /app

# Install any needed packages specified in requirements.txt
RUN python -m pip install --updagrade pip
COPY requirements.txt .
RUN pip install -r requirements.txt

COPY . .