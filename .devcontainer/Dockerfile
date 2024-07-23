FROM mcr.microsoft.com/dotnet/sdk:8.0

# Install additional dependencies if needed
RUN apt-get update && apt-get install -y \
    nodejs \
    npm \
    && rm -rf /var/lib/apt/lists/*

# Set the working directory
WORKDIR /workspace

# Copy the project files into the container
COPY . /workspace

# Install npm packages if needed
RUN npm install -g npm@latest
