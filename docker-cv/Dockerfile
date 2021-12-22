FROM debian:10.3

RUN apt-get update && apt-get install --yes --no-install-recommends \
    git \
    texlive-fonts-recommended \
    texlive-generic-recommended \
    texlive-latex-extra \
    texlive-fonts-extra \
    dvipng \
    texlive-latex-recommended \
    texlive-base \
    texlive-pictures \
    texlive-lang-cyrillic \
    texlive-science \
    cm-super \
    texlive-generic-extra \
    apt-get install texlive-bibtex-extra biber

RUN git clone https://github.com/yu432/testing_for_docker.git

RUN cd testing_for_docker/docker-cv/Simple-CV/ && pdflatex main.tex
CMD [ "bash" ]

