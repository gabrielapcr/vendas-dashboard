
Projeto Vendas – Dashboard com Filtros e Gráficos

Este projeto é uma aplicação web para visualização de dados de vendas. Possui autenticação simulada, gráficos de linha e barra com filtros por produto e data.


 Passos para instalação e execução

 Requisitos:
- Java 17 ou superior
- Node.js 18 ou superior
- Maven
- npm ou yarn

Backend (Spring Boot)
1. Navegue até a pasta do backend:
   cd vendas-api-backend

2. Inicie o servidor:
   mvn spring-boot:run

3. O backend será iniciado em http://localhost:8080

Frontend (React)
1. Navegue até a pasta do frontend:
   cd vendas-dashboard-frontend

2. Instale as dependências:
   npm install

3. Inicie o frontend:
   npm start

4. A aplicação abrirá automaticamente em http://localhost:3000


 Teste rápido da aplicação

1. Login automático:
   - Usuário: admin
   - Senha: senha123
   - Token salvo no localStorage como fake-token

2. Dashboard:
   - Gráfico de barras: Quantidade de vendas por produto
   - Gráfico de linhas: Evolução das vendas ao longo do tempo
   - Filtros: por data e por produto

3. Testar backend com curl:
   curl -H "Authorization: Bearer fake-token" http://localhost:8080/vendas


Tecnologias e bibliotecas utilizadas

Backend:
- Spring Boot 3.2.5 – Criação de APIs REST rápidas
- Spring Security – Controle de acesso com token fake
- CORS configurado – Integração com React frontend

Frontend:
- React – Interface dinâmica
- Recharts – Gráficos profissionais
- React Datepicker – Seleção de datas

 Observações finais

- Autenticação simulada com token "fake-token"
- Dados de vendas são simulados
- Componentes separados: Filtros, Gráficos e Dashboard
- Estilo limpo com cores azul claro, laranja e branco
* houve um problema na implementação final com o acesso do 'http://localhost:8080/vendas' from origin 'http://localhost:3000 que acabou culminando na não exibição dos dados

