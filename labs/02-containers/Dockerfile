FROM busybox:latest

ENV LOG /dev/null

CMD ["sh", "-c", "\
while true; do \
  echo \"$(hostname): $(date)\" | tee -a $LOG && \
  sleep 1; \
done"]