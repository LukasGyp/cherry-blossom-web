FROM python:3

WORKDIR /app

COPY requirements.txt ./
COPY main.py ./

RUN apt update && apt upgrade -y
RUN pip install --upgrade pip
RUN pip3 install --no-cache-dir -r requirements.txt

CMD [ "python3", "main.py" ]