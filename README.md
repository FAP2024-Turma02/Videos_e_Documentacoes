# Documentação de Instalação do Rails

## Introdução

Ruby on Rails, ou simplesmente Rails, é um framework web escrito em Ruby. Ele facilita o desenvolvimento de aplicações web seguindo o padrão MVC (Model-View-Controller). Esta documentação irá guiá-lo através do processo de instalação do Rails em um ambiente de desenvolvimento.

## Pré-requisitos

Antes de instalar o Rails, você precisa garantir que o Ruby esteja instalado no seu sistema. O Rails também requer algumas bibliotecas de sistema, que podem variar dependendo do sistema operacional. **Definido pelo professor vamos utilizar por padrão a versão 3.3.3 do Ruby.**

### Instalando Ruby

#### Windows

1. Baixe e instale o [RubyInstaller](https://rubyinstaller.org/).
2. Durante a instalação, certifique-se de marcar a opção "Add Ruby executables to your PATH".

#### macOS

1. Abra o Terminal.
2. Instale o Homebrew, se ainda não tiver:
   ```sh
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
3. Use o Homebrew para instalar o Ruby:
    ```sh
    brew install ruby
    ```
### Linux

1. Abra o terminal.
2. Instale as dependências necessárias.
    ```sh
    sudo apt-get update

    sudo apt-get install -y curl g++ gcc autoconf automake bison libc6-dev libffi-dev libgdbm-dev libncurses5-dev libsqlite3-dev libtool libyaml-dev make pkg-config sqlite3 zlib1g-dev libgmp-dev libreadline-dev libssl-dev
    ```
3. Instale o Ruby usando o RVM (Ruby Version Manager)
    ```sh
    \curl -sSL https://get.rvm.io | bash -s stable --ruby
    source ~/.rvm/scripts/rvm
    ```

## Instalando o Rails

1. Abra o terminal ou o prompt de comando.
2. Verifique se o Ruby está instalado corretamente.
    ```sh
    ruby -v
    ```
3. Instale o Bundler.
    ```sh
    gem install bundler
    ```
4. Instale o Rails.
    ```sh
    gem install rails
    ```
5. Verifique se o rails foi instalado corretamente.
    ```sh
    rails -v
    ```

## Configurando o Banco de Dados
O Rails utiliza por padrão o SQLite, mas você pode configurar outros bancos de dados como PostgreSQL ou MySQL.

### SQLite
O SQLite é instalado automaticamente com o Rails, portanto, nenhuma configuração adicional é necessária para usá-lo como banco de dados padrão. **Porém como definido em aula vamos utilizar o PostgreSQL**

## PostgreSQL
1. Instale o PostgreSQL
- Windows: Baixe e instale o PostgreSQL a partir do [Site Oficinal](https://www.postgresql.org/download/).
- macOS: Use o Homebrew para instalar:
 ```sh
 brew install postgresql
```
2. Configure o PostgreSQL seguindo as instruções de instalação.
 - [Link do vídeo de como instalar o PostgreSQL no windows](https://www.google.com/search?client=opera-gx&q=como+instalar+postgreSQL&sourceid=opera&ie=UTF-8&oe=UTF-8#fpstate=ive&vld=cid:8ab50539,vid:UbX-2Xud1JA,st:0).

## Criando um Novo Projeto Rails
1. No terminal, navegue até o diretório onde você deseja criar seu projeto.

2. Crie um novo projeto Rails(*`OBS` este comando não cria uma API com rails, e sim o projeto com rails*)
 ```
 rails new (nome_do_projeto)
 ```
3. Navegue até o diretório do projeto. 
 ```
 cd nome_do_projeto
 ```
4. Inicie o servidor Rails.
 ```
 rails server

 ou 

 rails s
 ```
5. Abra um navegador web e acesse http://localhost:3000. Você deve ver a página inicial padrão do Rails.

## Conclusão

Agora você tem o Ruby on Rails instalado e configurado no seu sistema. Você está pronto para começar a desenvolver suas aplicações web utilizando este poderoso framework. Para mais informações, consulte a [documentação oficial do Rails](https://guides.rubyonrails.org).

Este arquivo `README.md` em Markdown fornece uma orientação clara e detalhada sobre como instalar o Ruby on Rails.
