FROM alpine

RUN apk add curl

COPY smoke-test.sh smoke-test.sh

# Mend traceability labels
LABEL io.mend.identifier=9381fc9472d049b58c15c77103f182b705e1a3601f9b4027a7b289310d2b4e49
LABEL io.mend.image.dockerfile.path=master/test/smoke/Dockerfile
LABEL org.opencontainers.image.source=https://github.com/lukebrogan-mend/Demo

CMD ["sh", "smoke-test.sh", "http://app:3000"]
