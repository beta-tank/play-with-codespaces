FROM docker.io/zmkfirmware/zmk-dev-arm:3.0

RUN cd $LOCAL_WORKSPACE_FOLDER && \
    git clone --depth 1 --single-branch --branch=main https://github.com/zmkfirmware/zmk.git

COPY .bashrc tmp
RUN mv /tmp/.bashrc ~/.bashrc