<img src="https://elixir-lang.org/images/logo/logo.png" width="225" height="94">

# Next Level Week, trilha Elixir.

Trilha do evento Next Level Week na versão 4, desenvolvimento com programação funcional "Elixir". 

## Configuração do ambiente de desenvolvimento - Elixir

>Next Level Week 04, trilha Elixir🚀

Para começar o desenvolvimento em elixir com a programação funcional é necessário realizar alguns procedimentos para auxiliar no desenvolvimento da aplicação, algumas ferramentas fundamentais para o backend 💜

## Instação do Elixir e Phoenix
- Elixir
- Phoenix

## Instalação do Docker
- Windows (64 Bit)
- Windows (32 Bit)
- Mac OSX
- Linux (Ubuntu/Debian)

## Instação dos Postgres
- Com Docker
- sem Docker

# Instação do Elixir e Phoenix

#### Elixir
Para realizar a instação do Elixir, basta acessar o linl como pack na aula 01 e seguir os passos de acordo com o seu sistema operacional.

[Installing Elixir](https://elixir-lang.org/install.html)

Ao realizar a instalação eo Elixir com sucesso, você pode verificar se deu tudo certo rodando elixir - versão no terminal, Caso retorne algum erro, reinicie sua máquina e tente novamente o mesmo procedimento assim ou persistitm você pode seguir um recomendação de adicionar manualmente o Elixir nas configurações de opções de ambiente do seu sistema operacional. A seção(chamada Configurando a variável de ambiente PATH) está logo abaixo das instruções de download.

#### Phoenix

Com o Elixir instalado corretamente, basta instalar o framework Phoenix na sua máquina usando o seguinte comando:

```bash
mix archive.install hex phx_new 1.5.7
```

Você pode também acompanhar isso na documentação do Phoenix:

[Installation](https://hexdocs.pm/phoenix/installation.html#phoenix)

## Instação do Docker

O Docker é uma ferramenta sensacional que nos permite pular as etapas chatas de configuração de serviços para nossa aplicação. Além disso, ele permite reaproveitarmos o Kernel da máquina hospedeira entre vários serviços executados simultaneamente, conhecidos como containers.

Para iniciar a instalação do Docker vamos prosseguir para a seção "Get Started" presente no site da ferramenta:

[Get Started with Docker | Docker](https://www.docker.com/get-started)

### Windows (64 Bit)

O Docker no Windows possui alguns requisitos: 

- Microsoft Windows 10 Professional  ou Enterprise 64-bit
- Caso você possua o Windows 10 Home 64-bit também é possível usar o Docker mas será necessário instalar o WSL2 também (o instalador já se encarrega disso para você)

Caso tenha todos requisitos, então faça a instalação do Docker para Windows:

[Docker Desktop for Mac and Windows | Docker](https://www.docker.com/products/docker-desktop)

Depois de instalar o Docker e abrir o software você já está pronto para continuar. Lembrando que essa versão do Docker para Windows tem uma interface visual muito bacana, ou seja, você pode usar a interface para visualizar os serviços sendo executados, logs, imagens e muito mais.

Para verificar que o Docker foi instalado corretamente, em **uma nova janela** do terminal execute:

```bash
docker version
```

### Windows (32 Bit)

Infelizmente o Docker não possui suporte para sistemas 32 Bit, nesse caso é recomendável que você instale, manualmente, cada serviço (como o Postgres que será utilizado nessa trilha). 

Na [seção de instalação do Postgres](https://www.notion.so/Configura-es-do-ambiente-Elixir-f823443de76840cbbcb8ab1db8aa4667) deixaremos um link para que você possa ver uma alternativa de como instalar manualmente.

### Mac OSX

No MacOS o processo de instalação do Docker é extremamente simples, você precisa apenas baixar o app executável e executa-lo na máquina para iniciar o Docker:

[Docker Desktop for Mac - Docker Hub](https://hub.docker.com/editions/community/docker-ce-desktop-mac)

Depois de aberto você pode garantir que o Docker foi instalado corretamente executando o comando abaixo em uma nova janela do terminal:

```bash
docker version
```

### Linux (Ubuntu/Debian)

No Linux, vamos instalar o Docker utilizando o `apt`, para isso, em seu terminal, execute os comandos abaixo:

```bash
sudo apt update
sudo apt remove docker docker-engine docker.io
sudo apt install docker.io
```

Agora com o Docker instalado, vamos habilitar para que seu serviço seja iniciado automaticamente com o sistema:

sudo systemctl start docker
sudo systemctl enable docker

Para garantir que o Docker foi instalado da forma correta, execute no terminal:

```bash
docker version
```

Você precisará executar todos comandos do Docker utilizando o `sudo`, mas caso queira executa-los sem o `sudo`, utilize [esse guia](https://docs.docker.com/engine/install/linux-postinstall/#manage-docker-as-a-non-root-user).

## Instalação do Postgres

### Com Docker

Com o Docker instalado na sua máquina, basta rodar no terminal o comando:

```bash
docker run --name postgres -e POSTGRES_PASSWORD=postgres -p 5432:5432 -d postgres
```

Lembrando que caso você esteja usando Ubuntu/Debian é necessário usar `sudo` antes do comando.

### Sem Docker

Caso você esteja usando o Windows numa versão 32 Bit ou simplesmente não quer instalar o Docker na sua máquina, é possível realizar a instalação do postgres sem que dependa do Docker. Para isso basta acessar esse link, escolher a opção adequada para o seu sistema operacional e fazer a instalação como recomendado:

[Downloads](https://www.postgresql.org/download/)

>Documentação Oficial <https://elixir-lang.org/>








