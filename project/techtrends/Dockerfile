FROM python:2.7
LABEL maintainer="James Ononiwu"

COPY . /app
WORKDIR /app
RUN pip install -r ./project/techtrends/requirements.txt
RUN python  ./project/techtrends/init_db.py

# command to run on container start
CMD [ "python", "./project/techtrends/app.py" ]