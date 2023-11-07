# Projeto Jellyfin

Este é um projeto que usa o [Jellyfin], um sistema de mídia gratuito e de código aberto, para criar um servidor de streaming pessoal. Com o Jellyfin, você pode gerenciar, reproduzir e transmitir sua coleção de filmes, séries, músicas, podcasts e fotos para qualquer dispositivo.

## Funcionalidades

- Interface web amigável e responsiva
- Suporte a vários formatos de mídia, incluindo MP4, MKV, AVI, MP3, FLAC, etc.
- Transcodificação em tempo real para adaptar a qualidade do vídeo ao dispositivo e à rede
- Legendas integradas e externas
- Bibliotecas personalizáveis e organizadas por gênero, ano, diretor, etc.
- Controle parental e perfis de usuário
- Plugins para adicionar funcionalidades extras, como integração com o [Trakt], [OMDb], [TheTVDB], etc.
- Aplicativos nativos para Android, iOS, Roku, Fire TV, Apple TV, etc.

## Instalação

Para instalar o projeto, você precisa ter o [Docker] e o [Docker Compose] instalados no seu computador. Em seguida, siga os passos abaixo:

1. Clone este repositório para o seu computador usando o comando `git clone https://github.com/luciosilva/jellyfin`.
2. Entre na pasta do projeto usando o comando `cd projeto-jellyfin`.
3. Crie um arquivo chamado `.env` na raiz do projeto e adicione as seguintes variáveis de ambiente:

    ```env
    # O caminho onde você quer armazenar os dados do Jellyfin, como configurações, metadados, etc.
    JELLYFIN_DATA=/caminho/para/a/pasta/de/dados

    # O caminho onde você quer armazenar os arquivos de mídia, como filmes, séries, músicas, etc.
    JELLYFIN_MEDIA=/caminho/para/a/pasta/de/midia

    # A porta que você quer usar para acessar o Jellyfin pela web
    JELLYFIN_PORT=8096
    ```

4. Inicie o projeto usando o comando `docker-compose up -d`. Isso irá baixar a imagem do Jellyfin e criar um container para executá-lo.
5. Acesse o Jellyfin pela web usando o endereço `http://localhost:JELLYFIN_PORT`, onde `JELLYFIN_PORT` é a porta que você definiu no arquivo `.env`.
6. Siga o assistente de configuração inicial para criar um usuário administrador e adicionar as suas bibliotecas de mídia.
7. Aproveite o seu servidor de streaming pessoal!

## Contribuição

Se você quiser contribuir com este projeto, sinta-se à vontade para enviar um pull request ou abrir uma issue. Você também pode entrar em contato comigo.

## Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo [LICENSE] para mais detalhes.
