# Crear imagen = docker build -t centos-phoronix
# test = docker -it container_name bash; phoronix-test-suit [test]
FROM centos
RUN yum install git yum-utils php-cli php-xml zip -y
RUN git clone https://github.com/phoronix-test-suite/phoronix-test-suite.git
WORKDIR /phoronix-test-suite
RUN chmod u+x install-sh
RUN ./install-sh
