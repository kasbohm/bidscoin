Bootstrap: docker
FROM: python:3.7-slim

%help 
    Run bidstrainer.py, bidsmapper.py, bidscoiner.py

%files
    . /code       

%post
    chmod -R +x /code
    cd /code
    apt-get update && apt-get install -y --no-install-recommends git
    pip install --upgrade pip setuptools && pip install -r /code/requirements.txt && pip install -e .
    mkdir /tsd /usit /cluster /net
