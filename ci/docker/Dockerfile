FROM am-registry:5000/anothermemory/go-base

ADD glide.* /am/
RUN cd /am && \
    glide install --force --v && \
    mv /am/vendor/* /go/src && \
    cd /go/src && \
    rm -rf ./am