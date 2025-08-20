# Laboratório Prático AWS: Site Estático com S3 + CloudFront

Reforçando meus conhecimentos em **Cloud Computing**, realizei um laboratório prático para hospedagem de sites estáticos e distribuição de conteúdo via CDN na AWS.

<img width="1919" height="1079" alt="Siteestatico" src="https://github.com/user-attachments/assets/63950523-1d3b-46d8-9b8f-1e97c608d056" />

## Etapas do projeto

- Criação de um bucket no Amazon S3 e upload dos arquivos do site.
- Configuração de permissões para acesso público seguro.
- Criação de uma distribuição Amazon CloudFront para entrega global com baixa latência.
- Ajuste do **Default Root Object** no CloudFront para `index.html`, garantindo que a aplicação fosse exibida corretamente sem depender do Static Website Hosting do S3.

## Aprendizado importante

Durante o processo, percebi que, ao usar o endpoint padrão do S3 com CloudFront, é melhor desativar o **Static Website Hosting** e definir o `index.html` diretamente no CloudFront. Essa abordagem oferece melhor compatibilidade com HTTPS e é mais adequada para ambientes de produção.

## Tecnologias utilizadas

- Amazon S3
- Amazon CloudFront
- HTML, CSS e JavaScript (para o site estático)
