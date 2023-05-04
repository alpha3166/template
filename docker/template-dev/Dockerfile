FROM alpine
ARG USERNAME=me
RUN addgroup -g 1000 $USERNAME && \
    adduser -u 1000 -G $USERNAME -D $USERNAME
RUN apk -U add sudo && \
    echo "$USERNAME ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/$USERNAME
RUN apk -U add git less
USER $USERNAME
