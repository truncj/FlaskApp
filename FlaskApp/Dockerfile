FROM ubuntu:14.04

# Install PythonPip 
RUN apt-get -yqq update
RUN apt-get install -yqq python python-dev python-distribute python-pip

# Install Flask
RUN pip install flask

# Bundle app source
ADD . /src

# Expose
EXPOSE 5000

# Run
CMD ["python","/src/app.py"]
