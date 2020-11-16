FROM python:stretch

COPY . /main
WORKDIR /main


RUN pip install --upgrade pip
RUN pip install --no-cache-dir -r requirements.txt


ENTRYPOINT ["gunicorn", "-b", ":8080", "main:APP"]

