FROM opensearchproject/opensearch:latest

# Копируем все нужные конфигурационные файлы и сертификаты
COPY opensearch/opensearch.yml /usr/share/opensearch/config/opensearch.yml
COPY opensearch/certs/ /usr/share/opensearch/config/certs/

# Устанавливаем начальный пароль для admin пользователя
ENV OPENSEARCH_INITIAL_ADMIN_PASSWORD=CRCpFGDNe3

# Определяем точку входа
ENTRYPOINT ["/usr/share/opensearch/bin/opensearch"]
