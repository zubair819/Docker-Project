FROM nginx:latest

# remove default log symlinks
RUN rm -f /var/log/nginx/access.log \
    && rm -f /var/log/nginx/error.log

# create real log files
RUN touch /var/log/nginx/access.log \
    && touch /var/log/nginx/error.log

COPY nginx.conf /etc/nginx/nginx.conf