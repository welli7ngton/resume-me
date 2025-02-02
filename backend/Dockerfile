FROM python:3.10-alpine3.21

WORKDIR /app

COPY backend/ .

RUN pip install poetry

RUN poetry install --no-root

ENV PYTHONUNBUFFERED=1

CMD ["poetry", "run", "python", "backend/manage.py runserver"]
