bootstrap: docker
From: ubuntu:16.04

%labels
    Mamana Mbiyavanga "mamana.mbiyavanga@uct.ac.za", Ayton Meintjes "ayton.meintjes@uct.ac.za"

%help
    This container provides an installation of tools needed for the chipimputation pipeline
    on https://github.com/h3abionet/chipimputation

%environment
    export LANG=en_US.UTF-8
    export LANGUAGE=en_US:en
    export LC_ALL=C

%post
    # Update packages and install tools
    apt-get update -y && apt-get install -y wget git gcc g++ unzip make pkg-config

    # Install pip and python libs
    apt-get install -y python-dev python-setuptools python-pip build-essential libxml2-dev libxslt1-dev
    pip install --upgrade pip

    # Install cmake 3.2
    WORKDIR /tmp/cmake
    wget http://www.cmake.org/files/v3.2/cmake-3.2.2.tar.gz && tar xf cmake-3.2.2.tar.gz && cd cmake-3.2.2 && ./configure && make && make install

