FROM python:3.11-slim@sha256:a2bc8c35469b6fe37735f7c4dae39049470b2ce068e73f799c02452de31d24c6

COPY requirements.txt /app/
RUN pip install --no-cache-dir -r /app/requirements.txt

COPY manage.py /app/
COPY src/ /app/src/
WORKDIR /app/

RUN python manage.py migrate
RUN python manage.py loaddata src/fixtures.json
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
