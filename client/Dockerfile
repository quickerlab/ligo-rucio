FROM ligo/software:el7
MAINTAINER James Alexander Clark <james.clark@ligo.org>

# Install Rucio
# Based on https://github.com/rucio/rucio/blob/master/etc/docker/daemons/Dockerfile
RUN pip install rucio-clients

#   # Install dependencies for dataset creation
#   RUN yum install -y \
#       ldg-client \
#       wget \
#       gfal2 \
#       gfal2-plugin-file \
#       gfal2-plugin-gridftp \
#       gfal2-plugin-http \
#       gfal2-plugin-srm \
#       gfal2-plugin-xrootd \
#       gfal2-python
#
#   # PyCBC
#   RUN pip install --upgrade setuptools pip git+https://github.com/ligo-cbc/pycbc  

#RUN groupadd -r ligo-rucio && useradd --no-log-init -r -g ligo-rucio ligo-rucio
#USER ligo-rucio
WORKDIR /home/ligo-rucio

USER $USER

ENTRYPOINT ["/bin/bash"]


