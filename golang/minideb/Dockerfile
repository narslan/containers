FROM bitnami/minideb

LABEL authors="Nevroz Arslan"
 
ENV OS_ARCH="${TARGETARCH:-amd64}" \
    OS_FLAVOUR="debian-11" \
    OS_NAME="linux"\
    PATH="${PATH}:/usr/local/go/bin" \
    COMPONENT="go1.19.2.linux-amd64.tar.gz"

RUN apt update; apt -y install git g++ make curl pkg-config 

WORKDIR /tmp

RUN  curl -SsLf "https://go.dev/dl/${COMPONENT}" -o ${COMPONENT} && tar -C /usr/local -xzf ${COMPONENT} &&  rm -rf ${COMPONENT} ;
