FROM docker.io/zmkfirmware/zmk-dev-arm:3.0
ARG ZMK_URL
ARG ZMK_BRANCH
ARG ZMK_PATH

RUN git clone --depth 1 --single-branch --branch=${ZMK_BRANCH} ${ZMK_URL} ${ZMK_PATH}
RUN ls -la
COPY .bashrc tmp
RUN mv /tmp/.bashrc ~/.bashrc