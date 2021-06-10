## UFOP Opportunities - Sistema de Estágios

O software UFOP Opportunities tem por objetivo realizar a gestão dos processos de estágio na Universidade Federal de Ouro Preto.

## Dependências

Os requisitos mínimos para execução são:

- PHP 7.4
- [GD extension](http://php.net/manual/en/book.image.php)
- [PDO_PGSQL extension](https://www.php.net/manual/en/ref.pdo-pgsql.php)
- [ZIP extension](http://php.net/manual/en/book.zip.php)


## Instalação

### Execução via container

#### Docker

- Instale o [docker](https://docs.docker.com/get-started/)
- Instale o [docker-compose](https://docs.docker.com/compose/install/)


#### Instalando o projeto

- Clone o projeto para sua máquina: ``git clone git@github.com:UfopInternship/oportunidades.git``
- Crie um arquivo .env levando como base o .env.example na raiz do projeto.
- Compile e inicie os containers: `docker-compose build && docker-compose up -d`
- Instale as dependências do projeto a partir do container app. Execute o comando: ``docker-compose exec app composer install``.
- Gere as chaves de criptografia do Laravel: ``docker-compose exec app php artisan key:generate``
- Crie a chave de criptografia do projeto com o comando: ``php artisan key:generate``
- Execute as migrations com o comando: ``php artisan migrate``
- Povoe a base de dados com seeds executando: ``php artisan db:seed``
- Acesse com o navegador através do endereço: `http://localhost:8000`


## Contribuindo


## Vulnerabilidades conhecidas



## Licença


