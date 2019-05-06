Bootstrap: docker
FROM: python:3.7-slim

%help 
    Run bidstrainer.py, bidsmapper.py, bidscoiner.py

%files
    . /code       

%post
<<<<<<< HEAD
    chmod -R +x /code
=======
    chmod -r +x /code
>>>>>>> 7ac77003ee33b23a9ae27a046369eb3f0a95939b
    cd /code
    apt-get update && apt-get install -y --no-install-recommends git
    pip install --upgrade pip setuptools && pip install -r /code/requirements.txt && pip install -e .
    mkdir /tsd /usit /cluster /net
