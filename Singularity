bootstrap: docker
From: ubuntu:16.04

%labels
    Mamana Mbiyavanga "mamana.mbiyavanga@uct.ac.za", Ayton Meintjes "ayton.meintjes@uct.ac.za"

%help
    This container provides an installation of tools needed for the chipimputation pipeline
    on https://github.com/h3abionet/chipimputation

%environment
    export PATH=/opt/miniconda2/bin:$PATH

%post
    # Install Basic tools
    apt-get update && apt-get install -y \
        python python-dev python-pip \
        unzip \
        wget \
        pkg-config
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*