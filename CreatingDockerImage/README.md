# Criando uma imagem Docker

## 1. Tutorial overview

Esse tutorial irá guiá-lo pelo processo de criar uma imagem Docker, executá-la localmente e publicá-la no repositório de imagem.

Nesse tutorial assumiremos que você completou os passos para configurar o ambiente e possui os seguintes recursos já funcionado:

- Uma conta AWS.
- Cliente Git instalado.
- Docker Engine instalado.
- AWS CLI instalado e configurado.

Para checar se o cliente Git está instalado:

```
$ git --version
```

A saída será algo como:

```
$ git --version
git version 2.16.0.windows.2
```

Para checar se o Docker está instalado:

```
$ docker -v
```

A saída será algo como:

```
$ docker -v
Docker version 19.03.8, build afacb8b
```

Para checar se o AWS CLI está instalado:

```
$ aws --version
```

A saída será algo como:

```
$ aws --version
aws-cli/1.16.85 Python/3.6.0 Windows/10 botocore/1.12.75
```

> Lembre-se que para esse tutorial é recomendado ter instaldo a versão mais recente do AWS CLI.

Para checar o usuário configurado no AWS CLI:

```
$ aws iam get-user --output json
```

A saída será algo como:

```json
$ aws iam get-user --output json
{
    "User": {
        "Path": "/",
        "UserName": "dev.awscli",
        "UserId": "AWS_ACCESS_KEY_ID",
        "Arn": "arn:aws:iam::<account-id>:user/dev.awscli",
        "CreateDate": "2019-01-09T13:25:14Z",
        "Tags": [
            {
                "Key": "Name",
                "Value": "AwsCli"
            }
        ]
    }
}
```

> Para esse comando ser bem sucedido, as credências configuradas no AWS CLI devem ter permissão de leitura no AWS IAM.
