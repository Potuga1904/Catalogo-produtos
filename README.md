# 📦 Catálogo de Produtos – Serviços Web Multitecnologia

Projeto desenvolvido no âmbito da unidade curricular de Integração de Sistemas (IS), com o objetivo de implementar um sistema cliente-servidor multitecnologia, utilizando diferentes tipos de serviços Web: REST, SOAP, GraphQL e gRPC.

---

## 🎯 Objetivo

Desenvolver um catálogo de produtos com operações CRUD, suportando múltiplos formatos e protocolos, com capacidade de exportação/importação de dados em JSON e XML.

---

## 🧰 Tecnologias Utilizadas

### 🖥️ Servidor:
- **REST** com Flask
- **SOAP** com Spyne
- **GraphQL** com Graphene
- **gRPC** com gRPC Python
- Validação com JSON Schema e XSD
- Dados persistentes em ficheiros JSON
- Contêineres Docker orquestrados com Docker Compose

### 💻 Cliente:
- Python (linha de comandos)
- Bibliotecas: `requests`, `zeep`, `grpcio`, `gql`

---

## 📁 Estrutura do Projeto

atalogo-produtos/ ├── servidor/ │ ├── rest/ │ ├── soap/ │ ├── graphql/ │ ├── grpc/ │ └── dados/ # produtos.json ├── cliente/ # cliente Python ├── documentacao/ │ ├── schemas/ # JSON Schema / XSD │

Executar os serviços
docker compose up --build

4. Aceder aos serviços
REST	http://localhost:5000/produtos
SOAP	http://localhost:8000/?wsdl
GraphQL	http://localhost:5002/graphql
gRPC	Porta definida no .proto (ex: 50051)
