FROM python:3.10

ENV PYTHONUNBUFFERED=1

WORKDIR /tpc-core

COPY requirements.txt /tpc-core
RUN pip3 install -r requirements.txt --no-cache-dir

COPY . /tpc-core

ENTRYPOINT ["python3"]
CMD ["manage.py", "runserver", "0.0.0.0:8000"]
