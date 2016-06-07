# Use the latest Golang base image from the public Docker image repository
FROM golang

# Create app directory in the container
RUN mkdir -p /demo/app

# Set working directory in container to be the one we just created
WORKDIR /demo/app

# Copy app's source code from current directory to the directory we created in container
COPY . /demo/app

# Expose port 5000 so that it can be reached by the host
EXPOSE 5000

CMD ["go", "run", "helloworld.go"]
