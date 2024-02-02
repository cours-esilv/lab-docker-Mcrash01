# Use an official Python runtime as the base image
FROM python:3

# Set the working directory in the container
WORKDIR /app

# Copy the back part of the application code to the working directory
COPY . .

# Install dependencies
RUN pip install -r requirements.txt

# Expose the port the app runs on
EXPOSE 8080

# Command to run the application
CMD python3 -m flask run --host=0.0.0.0
