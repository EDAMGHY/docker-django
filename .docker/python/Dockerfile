# Use an official Python runtime as a parent image
FROM python:3.9

# Set environment variables for Python and Django
ENV PYTHONUNBUFFERED 1

# Create and set the working directory
WORKDIR /app

# Copy the requirements file into the container
COPY requirements.txt /app/

# Install dependencies
RUN pip install -r requirements.txt

# Copy the project code into the container
COPY . /app/

# Expose the port your Django app runs on (usually 8000)
EXPOSE 8000

# Run the Django development server
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
