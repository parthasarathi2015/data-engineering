FROM jupyter/pyspark-notebook:spark-3.4.1

# Set working directory
WORKDIR /home/jovyan/work

ENV MYSQL_ROOT_PASSWORD=password
ENV MYSQL_DATABASE=mydatabase

# Install Python packages 
COPY ./requirements.txt ./requirements.txt
RUN pip install -r requirements.txt

# Expose Jupyter port
EXPOSE 8888
