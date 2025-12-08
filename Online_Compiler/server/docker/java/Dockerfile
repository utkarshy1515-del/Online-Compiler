# Java Runtime Container
FROM eclipse-temurin:17-jdk-jammy

# Install essential tools
RUN apt-get update && apt-get install -y \
    coreutils \
    && rm -rf /var/lib/apt/lists/*

# Create app directory
WORKDIR /app

# Set security limits
RUN useradd -m -s /bin/bash coderunner
USER coderunner

# Default command
CMD ["/bin/bash"]