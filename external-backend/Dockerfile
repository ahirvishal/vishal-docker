FROM python:3.6

COPY ./requirements.txt .

RUN  pip install -r requirements.txt

ENV key=value

RUN [ "python3 manage.py collectstatic –noinput" ]

CMD [ "python3 manage.py makemigrations" && "python3 manage.py migrate" ]

ENTRYPOINT [ "executable" ] 
