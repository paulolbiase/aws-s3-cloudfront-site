# Laboratório Prático AWS: Site Estático com S3 + CloudFront

Reforçando meus conhecimentos em **Cloud Computing**, realizei um laboratório prático para hospedagem de sites estáticos e distribuição de conteúdo via CDN na AWS.

<img src="https://github.com/user-attachments/assets/f9b0d165-db37-477d-91be-d5b340cfb7e6" alt="Site Estático" width="650">


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

## Configurações da distribuição CloudFront

Segue um resumo das principais configurações que utilizei na distribuição:

![Configuração do Cloudfront](https://github.com/user-attachments/assets/7841829a-5522-4a32-8e9f-a8c953b1a869)
![Configuração do root object](https://github.com/user-attachments/assets/24b350e7-1cc7-4b49-82c0-f4765b29a938)

