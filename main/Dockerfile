FROM python:2.7
ENV PYTHONUNBUFFERED 1

# Create directories
RUN mkdir /code /code/client /code/server

WORKDIR /code

# install requirements
# do this before adding code so that if requirements stay the same, docker will
# not need to rebuild this part.
ADD server/requirements.txt /code/server/
RUN pip install -r server/requirements.txt

# Add code to /code on container
ADD . /code/