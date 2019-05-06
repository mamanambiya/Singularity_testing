bootstrap: docker
From: ubuntu:16.04

%labels
    Mamana Mbiyavanga "mamana.mbiyavanga@uct.ac.za", Ayton Meintjes "ayton.meintjes@uct.ac.za"

%help
    Simple Ubuntu 16.04 container for testing
    on https://github.com/h3abionet/chipimputation

%environment
    export LANG=en_US.UTF-8
    export LANGUAGE=en_US:en
    export LC_ALL=C

%post
    # Update packages and install tools
    apt-get update -y && apt-get install -y wget git gcc g++ unzip make pkg-config