FROM python:3.10-slim
# Set the working directory in the container
WORKDIR /app
# Copy the dependencies file to the working directory in the container
COPY requirements.txt .
# Install any dependencies and packages specified in requirements.txt and no caches are considered to reduce the image size
RUN pip install --no-cache-dir -r requirements.txt
# Copy the content of the local src directory to the working directory in the container
COPY . .
# port on which the container will listen for requests
EXPOSE 3000
# Run the application
CMD ["python", "main.py"]