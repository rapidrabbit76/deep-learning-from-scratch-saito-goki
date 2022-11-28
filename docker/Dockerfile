FROM python:3.11.0-slim
WORKDIR /ws

RUN apt-get update && apt install -y \ 
    libgl1-mesa-glx \
    curl  \
    git \ 
    vim \ 
    ranger \
    tmux \
    libglib2.0-0 && apt-get clean 

COPY ./requirements.txt /ws
RUN pip install --no-cache-dir -r requirements.txt