# Mentoria - API Laravel

## Diretórios

- src = Aplicação wordpress
- db = Arquivos do banco de dados (Local!!! Não subir para o git)
- DockerConfig = Arquivos de configuração do Docker

## Como rodar (1° passo)

### Levanta o ambiente (na raiz)

```bash
docker-compose up --build -d
```

### Durrubar o container (na raiz)

```bash
docker-compose down
```

### verifica se o container estar de pé

```bash
docker ps
```

### Acessando o container da aplicação

```bash
docker exec -it aula-laravel bash
```

### Instalando as dependencias

### (2° passo)

### Dentro da pasta src (no terminal aqui do vscode, digite cd src)

```bash

composer install
```

### Rodando as migrations

```bash
php artisan migrate
```

### Acessando a ROTA (Trocar {rota} pelo nome da rota criado)

```bash
localhost/api/{rota}
```

##############################################################################

#outros

### Acessando o container do Banco de Dados

```bash
docker exec -it db_agenda bash
```

### Se tiver problema no Windows

```
 --config core.autocrlf=input
```

### dicas

Ao criar uma função dentro do controller, sempre crie um rota para chamar aquela função
