# Use the official Nginx image as the base
FROM nginx:alpine

# Maintainer information
LABEL maintainer="HTML Codex"
LABEL template_name="Restoran - Bootstrap Restaurant Template"
LABEL template_link="https://htmlcodex.com/bootstrap-restaurant-template"
LABEL license="https://htmlcodex.com/license"
LABEL author_website="https://htmlcodex.com"

# Set the working directory to the Nginx web root
WORKDIR /usr/share/nginx/html

# Remove default Nginx files
RUN rm -rf ./*

# Copy project files to the container
COPY . .

# Expose port 80 for HTTP
EXPOSE 80

# Start Nginx when the container runs
CMD ["nginx", "-g", "daemon off;"]
