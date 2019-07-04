FROM adoptopenjdk/openjdk12-openj9:latest

RUN apt-get update && apt-get -y install wget unzip && \
    cd /usr/lib && \
    wget -q https://github.com/JetBrains/kotlin/releases/download/v1.3.40/kotlin-compiler-1.3.40.zip && \
    unzip kotlin-compiler-*.zip && \
    rm kotlin-compiler-*.zip && \
    rm -f kotlinc/bin/*.bat && \
    echo "Done!"

ENV PATH $PATH:/usr/lib/kotlinc/bin
