FROM nginx:1.25

# Remove o arquivo de configuração padrão do NGINX
RUN rm /etc/nginx/conf.d/default.conf

# Copia o novo arquivo de configuração do NGINX
COPY nginx.conf /etc/nginx/conf.d/

# Copia os arquivos de certificado SSL para o container
COPY certificate.crt /etc/ssl/certs/
COPY private_key.key /etc/ssl/private/
