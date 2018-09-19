Bootstrap: docker
From: docker://quay.io/h3abionet_org/impute2

%labels
Mamana Mbiyavanga "mamana.mbiyavanga@uct.ac.za"

%post
    # Install Basic tools
    apt-get update && apt-get install -y \
        autoconf \
        build-essential \
        git \
        libncurses5-dev \
        pkg-config \
        unzip \
        wget \
        zlib1g-dev &&
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
