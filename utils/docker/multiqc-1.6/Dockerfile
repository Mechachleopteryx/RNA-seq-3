FROM conda/miniconda3-centos7

LABEL description="Docker image containing all requirements for RNA-seq pipeline"

RUN conda config --add channels defaults && conda config --add channels conda-forge && conda config --add channels bioconda
RUN conda install -y python=2.7.16 
RUN conda install -y bioconda::multiqc=1.6 && conda clean -a 

ENV LANG=en_US.UTF LC_ALL=en_US.UTF-8 
