FROM python:3.10-slim@sha256:d8e262e069903a0b7790cd17a66d5343b2f04b9d9e19dc70f152c50fb511acfe

WORKDIR /app

COPY ./test/data/redirect_reflect_app/requirements.txt requirements.txt
RUN pip install -r requirements.txt

EXPOSE 5000

CMD ["python", "app.py"]
