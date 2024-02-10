# Use an official Python runtime as the base image
FROM nginx

# Set the working directory in the container
WORKDIR /app

# Copy the back part of the application code to the working directory
COPY . .

# Set environment variable for backend URL
ENV WS_BACK_URL=http://host.docker.internal:8080

# Expose port 80
EXPOSE 80

# Use exec form for entrypoint
ENTRYPOINT ["nginx", "-g", "daemon off;"] # start Nginx as principal processus of the container (instead of daemon)
