FROM ubuntu:16.04 

WORKDIR /mydir
COPY . /mydir 
RUN apt-get update && apt-get install -y curl  
CMD ["sh","script.sh"]
