# Use the official Tomcat base image
FROM tomcat:9.0

# Optional: Remove default web apps to keep the image lightweight
RUN rm -rf /usr/local/tomcat/webapps/*

# Copy your application WAR file to the Tomcat webapps directory
# Replace `your-app.war` with the name of your WAR file
COPY your-app.war /usr/local/tomcat/webapps/

# Expose Tomcat port (default is 8080)
EXPOSE 8080

# Start Tomcat server
CMD ["catalina.sh", "run"]
