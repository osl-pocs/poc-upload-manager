FROM minio/minio:latest

ENV PATH=/opt/bin:$PATH

# COPY ./minio /opt/bin/minio
COPY containers/scripts/docker-entrypoint.sh /usr/bin/docker-entrypoint.sh

ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]

VOLUME ["/data"]

CMD ["minio"]