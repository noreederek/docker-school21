FROM python:3.7.3-slim

WORKDIR /data
COPY . /data
RUN pip install jupyter numpy matplotlib seaborn pandas
EXPOSE 8888
CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root"]
# docker run --rm -it -p 8888:8888 -v "$(pwd):/data" dsenv  