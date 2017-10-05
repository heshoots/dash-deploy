FROM java:alpine

RUN wget http://archive.apache.org/dist/jena/binaries/jena-fuseki1-1.6.0-distribution.zip
RUN unzip ./jena-fuseki*
RUN rm *.zip
RUN mv jena-fuseki1-1.6.0 /fuseki
WORKDIR /fuseki
CMD ./fuseki-server --update --mem /ds
