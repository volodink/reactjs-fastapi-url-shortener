FROM python:3.10

WORKDIR /backend

COPY requirements.txt .

# Installing python dependencies
RUN pip install -r requirements.txt

COPY src ./src
COPY .env .

CMD ["uvicorn", "src.main:app", "--reload", "--host", "0.0.0.0"]
# CMD ["ls", "-all"]
