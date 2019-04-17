# Set Version
ARG VERSION=2.4

FROM httpd:$VERSION

LABEL maintainer="Dmytro Melnyk"


COPY testFile.txt /usr/local/apache2/

RUN mkdir /mydata

RUN echo "test" > /mydata/image_test

#VOLUME /mydata


# Forward port to 8080
EXPOSE 8080


