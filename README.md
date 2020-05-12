# AWS Hands On - Docker, ECS, Git

## Configurando o ambiente

Para realizar as atividades desse _hands on_ será necessária uma conta na Amazon Web Services (AWS) e os seguintes utilitários instalados em sua máquina:

1. Um cliente Git.
2. Docker Engine.
3. AWS CLI.

> :star: Os recursos utilizados nesse _hands on_ estão dentro do limite de _free tier_ para um conta AWS com menos de 12 meses de criação.

### Criando uma conta AWS

Para realizar as atividades do hands on será necessária uma conta AWS ou um usuário IAM de uma conta AWS.

Assim, caso ainda não possua sua conta, siga os passos na página oficial da AWS sobre como criar uma nova conta.

**Para cadastrar-se na AWS**

1. Abra https://portal.aws.amazon.com/billing/signup
2. Siga as instruções online.
   > Parte do procedimento de cadastro envolve uma chamada telefônica e a digitação de um código de verificação usando o teclado do telefone

### Instalando o Git

Download e instalação: https://git-scm.com/downloads

Mais informações sobre Git: https://git-scm.com/book/en/v1/Getting-Started

### Instalando Docker

Docker roda nativamente em Mac, Windows e Linux.
Este laboratório irá usar o [Docker Community Edition - CE](https://www.docker.com/products/container-runtime).
Para instalar o Docker Engine e CLI em seu computador, por favor, siga os passos na [documentação oficial](https://docs.docker.com/engine/install/).
Você também pode instalar por distribuição Linux, por exemplo, para [Ubuntu](https://docs.docker.com/engine/install/ubuntu/).

### Instalando o AWS CLI

Durante o _hands on_ vamos interagir com albumas AWS API's.
Instalar a versão mais recente do AWS CLI será o mais apropriado.

Instalando AWS CLI: https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html

Configurando AWS CLI: https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html#cli-quick-configuration

### Clonando o reposítorio do workshop

Para clonar este repositório, você pode usar o seguinte comando:

```
$ git clone https://github.com/vinicius-lima/aws-hands-on-docker-ecs-git.git
```

Após clonar o repositório, você verá que uma nova pasta chamada `aws-hands-on-docker-ecs-git` foi criada.
Todo o conteúdo do workshop está disponível nessa pasta.
