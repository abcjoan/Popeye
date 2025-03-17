FROM python:3.12
EXPOSE 80
WORKDIR /app
COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt
COPY . .
ENV FLASK_APP=app.py
CMD ["flask", "run", "--host=0.0.0.0", "--port=80"]