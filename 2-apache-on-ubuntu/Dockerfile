FROM ubuntu:latest
# Set the working directory
WORKDIR /usr/local/apache2

# Update the package list and install Apache
RUN apt-get update && apt-get install -y apache2 apache2-utils

# Expose port 80 for HTTP traffic
EXPOSE 80

# Start Apache in the foreground
CMD ["apache2ctl", "-D", "FOREGROUND"]