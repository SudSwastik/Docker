# Use existing docker image as a base
FROM alpine

# Download and Install Dependency
RUN apk add --update redis

# Command to run when container starts up
CMD ["redis-server"]

