FROM python:3.9-slim

#set workdir 
WORKDIR /app

COPY requirements.txt ./

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

ENV Flask_APP=app.py

EXPOSE 5000

CMD ["flask", "run", "-h", "0.0.0.0", "-p 5000"]