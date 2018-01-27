# Crear imagen = docker build -t debian-phoronix
# test = docker -it container_name bash; phoronix-test-suit [test]
FROM debian
RUN apt-get update -y
RUN apt-get install apt-utils git php-cli php-xml zip -y
RUN git clone https://github.com/phoronix-test-suite/phoronix-test-suite.git
WORKDIR /phoronix-test-suite
RUN chmod u+x install-sh
RUN ./install-sh
