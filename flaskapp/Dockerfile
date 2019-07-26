# The container starts from python 3 image
FROM python:3

# Set the main directory into the container
WORKDIR /usr/src/app

# Copy the local file requirements.txt that contains the python project dependencies
COPY requirements.txt ./

# install the dependencies copied above in the contaiter
RUN pip install --no-cache-dir -r requirements.txt

# Copy all files in the current directory into the main directory of the container
COPY . .

# Open port 5000 of the container (or something like that...)
EXPOSE 5000

# This is the command that will be run when the container start (launch the app.py file)
CMD ["python", "./app.py"]
