FROM python3

COPY ./requirements.txt .

RUN  pip install -r requirements.txt

ENV key=value

CMD [ "python3 manage.py makemigrations" && "python3 manage.py migrate" ]

ENTRYPOINT [ "executable" ] 
