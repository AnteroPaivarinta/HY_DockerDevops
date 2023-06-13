# Start from the alpine image
FROM ubuntu:20.04
RUN apt-get update && apt-get install -y curl 
# Use /usr/src/app as our workdir. The following instructions will be executed in this location.

# Copy the hello.sh file from this location to /usr/src/app/ creating /usr/src/app/hello.sh.
COPY 1.7.sh .

# Execute a command with `/bin/sh -c` prefix.
RUN chmod +x 1.7.sh
# When running Docker run the command will be ./hello.sh
CMD ./1.7.sh
