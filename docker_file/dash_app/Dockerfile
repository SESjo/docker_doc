FROM python:3.8-slim
COPY ./app /app
WORKDIR /app
RUN apt-get update
RUN apt-get install -y gdal-bin libgdal-dev g++
RUN python -m pip install --no-cache-dir --upgrade pip
RUN pip install protobuf==3.20.*
RUN pip install geopandas
RUN pip install dash-bootstrap-components
RUN pip install dash-extensions
RUN pip install dash-leaflet
RUN pip install pandas
RUN pip install dash
RUN pip install plotly
EXPOSE 8050
CMD ["python", "app.py"]
