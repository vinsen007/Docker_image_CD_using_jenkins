FROM redhat/ubi8
RUN yum install python -y
RUN pip install flask
COPY app.py /app.py
CMD [ "python", "/app.py" ]
