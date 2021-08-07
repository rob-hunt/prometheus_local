FROM ruby:2.5.1

ENV PROMETHEUS_EXPORTER_PORT 9394

RUN gem install prometheus_exporter -v 0.7.0
EXPOSE 9394

COPY ./entrypoint.sh .

CMD ["/entrypoint.sh"]
