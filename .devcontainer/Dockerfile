FROM ghcr.io/philips-software/amp-devcontainer:latest

# Install debugging tools
RUN apt-get update && apt-get install -y \
    gdb-multiarch \
    && rm -rf /var/lib/apt/lists/*

# Set the working directory
WORKDIR /workspace

# Copy the project files into the container
COPY . .

CMD ["bash"]