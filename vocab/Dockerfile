FROM python:3
MAINTAINER Willow Sack "willow0@uoregon.edu"
RUN apt-get update -y
RUN apt-get update && apt-get install -y python3-pip python3-dev build-essential 
#had to change above python install because of build issues
COPY . /app
WORKDIR /app
RUN pip install -r requirements.txt
ENTRYPOINT ["python"]
CMD ["flask_vocab.py"]
#RUN apt-get install -y python3-pip python-dev build-essential