# Use the base image for KrakenD
FROM devopsfaith/krakend:2.7.0

# Create the configuration directory
RUN mkdir -p /etc/krakend

# Copy the krakend.json file into the container
COPY krakend.json /etc/krakend/krakend.json

# Expose the necessary port
EXPOSE 8080

# Command to run the service with the configuration file
CMD ["krakend", "run", "-c", "/etc/krakend/krakend.json"]
