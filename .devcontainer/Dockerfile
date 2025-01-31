FROM ghcr.io/philips-software/amp-devcontainer:latest

# Install debugging tools
RUN apt-get update && apt-get install -y \
    gdb-multiarch \
    iproute2 \
    && rm -rf /var/lib/apt/lists/*

# Set the working directory
WORKDIR /workspace

# Copy the project files into the container
COPY . .

# Make sure the script is executable
RUN chmod +x scripts/get-wsl-ip.sh

CMD ["bash"]