FROM conda/miniconda3-centos7

LABEL description="Docker image containing all requirements for RNA-seq pipeline"

RUN conda config --add channels defaults && conda config --add channels conda-forge && conda config --add channels bioconda
RUN conda install -y bioconda::bowtie2=2.2.5 && conda clean -a 

ENV LANG=en_US.UTF LC_ALL=en_US.UTF-8 
