FROM ubuntu:latest

# Install vsftpd
RUN apt-get update && apt-get install -y vsftpd

# Copy the vsftpd configuration file
COPY vsftpd.conf /etc/vsftpd.conf

# Expose the FTP port
EXPOSE 20 21

# Run vsftpd in the foreground
CMD ["vsftpd", "/etc/vsftpd.conf"]
