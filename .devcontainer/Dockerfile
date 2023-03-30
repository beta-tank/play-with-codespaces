FROM docker.io/zmkfirmware/zmk-dev-arm:3.0
ARG LOCAL_WORKSPACE_FOLDER
ARG ANOTHER

RUN echo ${ANOTHER}
RUN echo ${LOCAL_WORKSPACE_FOLDER}
RUN ${LOCAL_WORKSPACE_FOLDER} dirname ${LOCAL_WORKSPACE_FOLDER}
RUN echo ${LOCAL_WORKSPACE_FOLDER}
RUN cd ${LOCAL_WORKSPACE_FOLDER} && \
    git clone --depth 1 --single-branch --branch=main https://github.com/zmkfirmware/zmk.git
RUN pwd
RUN ls -la
COPY .bashrc tmp
RUN mv /tmp/.bashrc ~/.bashrc