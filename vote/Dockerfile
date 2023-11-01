FROM python:3.11.6-alpine3.18
WORKDIR /vote
COPY . .
RUN pip install -r requirements.txt
EXPOSE 8080
CMD ["python", "app.py"]