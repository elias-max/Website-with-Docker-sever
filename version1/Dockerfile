# Use an official nginx image as a parent image
FROM nginx:alpine
 
# Set the working directory to /usr/share/nginx/html
WORKDIR /usr/share/nginx/html
 
# Copy the current directory contents into the container at /usr/share/nginx/html
COPY index.html .
 
# Expose port 80
EXPOSE 80
 
# Define the command to run the application
CMD ["nginx", "-g", "daemon off;"]