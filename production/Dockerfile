# syntax=docker/dockerfile:1

FROM rasa/rasa:3.5.1-spacy-en
COPY endpoints.yml endpoints.yml
COPY config.yml config.yml 
CMD ["run", "--endpoints", "endpoints.yml", "--cors", "*"]
EXPOSE 5005


############################################################
# build and run the container
# (with or without docker compose)
############################################################

############### using docker compse

## build image and rund the container
# docker compose up

## stop the container
# docker compose down


############### or NOT using docker compose

## build the docker image named 'tubafbot:chatbotbrain'
# docker build -t tubafbot:chatbotbrain --rm . 

## run the container
# docker run -p 5005:5005 tubafbot:chatbotbrain

## stop and remove the container
# docker rm $(docker stop $(docker ps -a -q --filter ancestor=tubafbot:chatbotbrain))

## remove the docker image from the repository
# docker image rm tubafbot:chatbotbrain
