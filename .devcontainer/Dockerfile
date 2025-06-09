
FROM ubuntu as base
RUN apt-get -y update
RUN apt-get -y install build-essential
RUN apt-get -y install rsync zip openssh-server
RUN apt-get -y install git tmux
RUN apt-get -y install curl wget
RUN apt-get -y install python3
RUN apt-get -y update && apt-get install -y python3-pip python3-venv
RUN apt-get install -y libffi-dev libssl-dev
RUN python3 -m venv /opt/venv
RUN /opt/venv/bin/pip install ipython
ENV PATH="/opt/venv/bin:$PATH"

RUN apt-get clean