FROM python:3.10-alpine

EXPOSE 8000

WORKDIR /app 

# COPY requirements.txt /app

# RUN pip install --upgrade pip
# RUN pip install -r requirements.txt --no-cache-dir
RUN pip install Django

COPY . /app 

EXPOSE 8000

# ENTRYPOINT ["python3"] 

CMD ["sh", "-c", "python manage.py makemigrations && python manage.py migrate && python manage.py runserver 0.0.0.0:8000"]