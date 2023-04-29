FROM python:3.9-slim
# TODO change the base images but 
COPY application_default_credentials.json application_default_credentials.json
ENV GOOGLE_APPLICATION_CREDENTIALS=/application_default_credentials.json

COPY requirements.txt requirements.txt 
RUN pip install --upgrade pip
RUN pip install -r requirements.txt 