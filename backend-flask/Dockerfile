FROM python:3.10-slim-buster

#Inside container
#make a new dir inside container
WORKDIR /backend-flask

#Outside container -> Inside container
#this contains the libraries to install to run the app
COPY requirements.txt requirements.txt

#Inside container
#install the python libraries used for the app
RUN pip3 install -r requirements.txt

#Outside container -> Inside container
#first period = everything in /backend-flask outside container
#second period = everything in /backend-flask inside container
COPY . .

#Inside container
#Set environment variables
#will remain set when the container is running
ENV FLASK_ENV=development

EXPOSE ${PORT}
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]
