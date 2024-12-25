# Assessment2

Step 1: Create a Simple Python Program Created a file named hello.py with the following content in VS

python print("Hello cloud-engine labs!!")

Step 2: Create a Dockerfile Created a file named Dockerfile in the same directory as your hello.py file with the following content:

Dockerfile Use an official Python runtime as a parent image FROM python:3.8-slim

Set the working directory in the container WORKDIR /app

Copy the current directory contents into the container at /app COPY . /app

Run hello.py when the container launches CMD ["python", "hello.py"]

Step 3: Test the Dockerfile by Building the Image Run the following command to build the Docker image: 

Right click on the Docker file and click build image

Step 4: Run the Image as a Container Run the following command to start a container from the image: bash docker run assessment

Step 5: Commit and Push the Updated Code into Your GitHub Repo bash git init

bash git add . Commit the Changes:

bash git commit -m "Add hello.py and Dockerfile"

bash git remote add origin https://github.com/Harish-365/Assesment2 Push the Changes to GitHub:

bash git push -u origin main
