# Repository Management System - Back-end

O projeto Repository Manager consiste em um sistema backend dividido em dois serviços principais, projetados para buscar, gerenciar e armazenar dados de usuários do GitHub. Os dois serviços são integrados utilizando mensageria RabbitMQ e estão encapsulados em containers Docker para facilitar a implantação e a escalabilidade.

## Pré-requisitos

Certifique-se de ter as seguintes dependências instaladas antes de iniciar:

- [Node.js](https://nodejs.org/) (versão 16.17.0 ou superior)
- Pacotes [npm](https://www.npmjs.com/) (Node Package Manager)
- [Docker](https://docs.docker.com/engine/install/)

## Instruções de Configuração

1. Clone o repositório com seus submodulos

```bash
git clone --recurse-submodules https://github.com/JoseEduardoMartins/repository-manager-backend.git

cd repository-manager-backend
```

2. Vá até o subrepositório repository-manager-backend-a e instale as dependencias

```bash
cd ./repository-manager-backend-a

npm install
```

3. Volte para raiz do projeto

```bash
cd ../
```

4. Vá até o subrepositório repository-manager-backend-b e instale as dependencias

```bash
cd ./repository-manager-backend-b

npm install
```

5. Configure as variáveis de ambiente no arquivo "docker-compose.yml".

6. Inicie o microserviço:

```bash
docker-compose up --build
```

Os servidores estarão disponíveis em http://localhost:3000 e http://localhost:3001 por default.

## Contribuição

Contribuições são bem-vindas! Se encontrar algum problema ou tiver sugestões, por favor, abra uma [issue](https://github.com/JoseEduardoMartins/customer-manager-backend/issues/new).

## Autor

- José Eduardo Martins

## Licença

Este projeto é licenciado sob a Licença MIT - consulte o arquivo LICENSE.md para obter detalhes.

## Contato

Para qualquer dúvida ou problema, entre em contato com `m4rt1ns.jose@gmail.com`.
