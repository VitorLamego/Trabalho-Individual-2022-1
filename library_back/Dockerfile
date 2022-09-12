FROM python:3

ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1

WORKDIR /library_back
COPY ./ ./

RUN pip install -r library_back/requirements.txt

ADD ./library_back/docker-entrypoint.sh ./docker-entrypoint.sh

RUN chmod a+x ./docker-entrypoint.sh
ENTRYPOINT ["./docker-entrypoint.sh"]

COPY . /code/
