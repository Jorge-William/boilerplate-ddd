# boilerplate-ddd
Scaffold para acelerar o desenvolvimento backend usando Domain Driven Design


### Descrição das Pastas

#### `/src`

Esta é a pasta principal que contém todo o código fonte do projeto.

- **/application**: Contém a lógica da aplicação, incluindo casos de uso e Data Transfer Objects (DTOs).
  - **/usecases**: Implementações dos casos de uso, como `DepositarDinheiro`, `SacarDinheiro`, e `ConsultarSaldo`.
  - **/dto**: Define objetos que são transferidos entre as camadas.

- **/core**: O núcleo da aplicação, onde reside a lógica de domínio.
  - **/entities**: Representa as entidades principais do sistema, como `Conta` e `Cliente`.
  - **/repositories**: Interfaces que definem métodos para acesso a dados persistidos.
  - **/services**: Contém serviços que implementam a lógica de negócios.

- **/infrastructure**: Adaptadores que conectam a aplicação ao mundo externo.
  - **/adapters**: Implementações que permitem a comunicação com bancos de dados ou APIs externas.
  - **/config**: Configurações necessárias para a infraestrutura, como conexão com o banco de dados.

- **/interfaces**: Define as portas que permitem a comunicação entre a camada de aplicação e a infraestrutura.

#### `/tests`

Contém testes unitários e de integração para garantir que todas as partes do sistema funcionem corretamente. É uma boa prática manter testes organizados por camada.

## Como Usar

1. Clone o repositório:
    ```
    git clone https://github.com/boilerplate-ddd.git
    cd boilerplate-ddd
    ```

2. Instale as dependências:
    ```
    npm install
    ```

3. Execute os testes:
    ```
    npm test
    ```

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests.

## Licença

Este projeto está licenciado sob a MIT License. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
