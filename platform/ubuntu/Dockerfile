FROM registry.gitlab.steamos.cloud/steamrt/steamrt4/sdk  AS base-image

RUN apt update -y
RUN apt install -y build-essential
RUN apt install -y cmake
RUN apt install -y git
RUN apt install -y python3
RUN apt install -y python3-pip
RUN apt install -y zip
RUN apt install -y curl
RUN apt install -y unzip
RUN apt install -y pkg-config
RUN apt install -y autoconf
RUN apt install -y libtool
RUN apt install -y flex
RUN apt install -y bison

FROM registry.gitlab.steamos.cloud/steamrt/steamrt4/sdk
COPY --from=base-image / /
