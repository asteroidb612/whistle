FROM balenalib/raspberrypi3
COPY Makefile Makefile
COPY whistle_control.c whistle_control.c
RUN apt-get -y update && apt-get -y install build-essential libfftw3-dev libasound2-dev
RUN make
RUN ./whistle_control
