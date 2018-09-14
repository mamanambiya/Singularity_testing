#######################################################################
#
# This container provides an installation of tools needed for the chipimputation pipeline.
#
# Changelog
# ---------
#
#######################################################################

bootstrap: docker
From: ubuntu:16.04

%labels
    Mamana Mbiyavanga "mamana.mbiyavanga@uct.ac.za"

%help
    This container provides an installation of tools needed for the chipimputation pipeline
    on https://github.com/h3abionet/chipimputation

%post
    # Install Basic tools

    # Install wget
    apt-get update && apt-get install -y \
      autoconf \
      build-essential \
      git \
      libncurses5-dev \
      pkg-config \
      unzip \
      wget \
      zlib1g-dev && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

    # Install IMPUTE2
    wget http://mathgen.stats.ox.ac.uk/impute/impute_v2.3.2_x86_64_static.tgz && \
        tar -zxvf impute_v2.3.2_x86_64_static.tgz && \
        mv impute_v2.3.2_x86_64_static/impute2 /usr/local/bin/impute2 && \
        mkdir /opt/impute2/example -p && \
        mv impute_v2.3.2_x86_64_static/Example/* /opt/impute2/example && \
        rm -rf impute_v2.3.2_x86_64_static impute_v2.3.2_x86_64_static.tgz


%environment
    export LANG=en_US.UTF-8
    export LANGUAGE=en_US:en
    export LC_ALL=en_US.UTF-8
    export PATH=/opt/miniconda3/bin:$PATH
    export XDG_RUNTIME_DIR=""
