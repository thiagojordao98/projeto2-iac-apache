Instalação e Configuração do Servidor Web
=========================================

Este script shell automatiza o processo de atualização do servidor e instalação do servidor web Apache. Ele também baixa e copia os arquivos da aplicação para o diretório `/var/www/html/`, tornando-os acessíveis por meio do navegador.

Pré-requisitos
--------------

Este script deve ser executado em um sistema Linux que tenha acesso à internet e permissões de root.

Instalação
----------

1.  Clone este repositório em seu sistema Linux usando o comando `git clone https://github.com/thiagojordao98/linux-iac/tree/main/projeto2-iac-apache`
2.  Acesse o diretório do repositório usando o comando `cd projeto2-iac-apache`
3.  Dê permissão de execução ao arquivo `iac-2.sh` usando o comando `chmod +x iac-2.sh`
4.  Execute o arquivo `iac-2.sh` usando o comando `./iac-2.sh`

Processos do script
----------

O script shell automatiza os seguintes processos:

1.  Atualização do sistema operacional usando o comando `apt-get update`.
2.  Atualização dos pacotes instalados no sistema operacional usando o comando `apt-get upgrade -y`.
3.  Instalação do servidor web Apache usando o comando `apt-get install apache2 -y`.
4.  Instalação do unzip usando o comando `apt-get install unzip -y`.
5.  Download dos arquivos da aplicação usando o comando `wget https://github.com/denilsonbonatti/linux-site-dio/archive/refs/heads/main.zip`.
6.  Descompactação dos arquivos usando o comando `unzip main.zip`.
7.  Copia dos arquivos para o diretório do servidor web usando o comando `cp -R * /var/www/html/`.

Após a execução do script, os arquivos da aplicação estarão acessíveis por meio do navegador em `http://localhost`.


