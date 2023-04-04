# Start from the alpine image
FROM ubuntu:latest 

# Use /usr/src/app as our workdir. The following instructions will be executed in this location.
WORKDIR /usr/src/app

# Copy the hello.sh file from this location to /usr/src/app/ creating /usr/src/app/hello.sh.
COPY curler.sh .

# Install curl
RUN apt update && apt install -y curl

# Add permissions
RUN chmod +x curler.sh

# When running Docker run the command will be ./hello.sh
CMD ./curler.sh