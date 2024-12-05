# Step 1: Define a base image with Python 3.9
FROM python:3.9-slim

# Step 2: Set the working directory inside the container
WORKDIR /app

# Step 3: Copy the requirements file (you can create this file later)
COPY requirements.txt /app/

# Step 4: Install any dependencies listed in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Step 5: Copy the entire application code to the container
COPY . /app/

# Step 6: Expose port 5000 for the Flask app
EXPOSE 5000

# Step 7: Set the default command to run the Flask app
CMD ["python", "app.py"]
