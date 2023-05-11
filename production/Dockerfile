# syntax=docker/dockerfile:1

FROM rasa/rasa:3.5.1-spacy-en
COPY endpoints.yml endpoints.yml
COPY config.yml config.yml 
CMD ["run", "--endpoints", "endpoints.yml"]
EXPOSE 5005

# build the container named 'tubafbot:chatbotbrain'
# docker build -t tubafbot:chatbotbrain --rm . 

# run the container
# docker run -p 5005:5005 tubafbot:chatbotbrain