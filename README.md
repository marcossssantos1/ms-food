🍔 ms-food
O ms-food é um sistema de microserviços desenvolvido em Java com o framework Spring Boot, projetado para gerenciar pedidos e pagamentos em uma aplicação de entrega de alimentos. Este projeto visa demonstrar a arquitetura de microserviços utilizando o Spring Cloud e o Eureka Server para descoberta de serviços.

🚀 Tecnologias Utilizadas
Java 21

Spring Boot 3.4.5

Spring Cloud 2024.0.1 (Camel)

Eureka Server (Service Discovery)

Maven Wrapper (mvnw)

Docker (para conteinerização)

MySQL (banco de dados relacional)

🧱 Estrutura do Projeto
O projeto está organizado em múltiplos microserviços, cada um responsável por uma funcionalidade específica:

eureka-server: Servidor Eureka para registro e descoberta de serviços.

pagamentos: Microserviço responsável pelo processamento de pagamentos.

pedidos: Microserviço responsável pela gestão de pedidos.

gateway: API Gateway para roteamento de requisições.
Reddit

⚙️ Configuração e Execução
Pré-requisitos
Java 21 instalado e configurado.

Docker instalado (opcional, para execução de contêineres).

MySQL em execução (caso não utilize Docker).

Passos para Execução
Clone o repositório:

bash
Copiar
Editar
git clone https://github.com/marcossssantos1/ms-food.git
cd ms-food
Inicie o servidor Eureka:

bash
Copiar
Editar
cd eureka-server
./mvnw spring-boot:run
Inicie os microserviços:

bash
Copiar
Editar
cd ../pagamentos
./mvnw spring-boot:run

cd ../pedidos
./mvnw spring-boot:run
Acesse o Eureka Dashboard:

URL: http://localhost:8081/eureka

🛠️ Configuração do IntelliJ IDEA
Para garantir que o projeto funcione corretamente no IntelliJ IDEA:

Abra o projeto no IntelliJ IDEA.

Vá em File > Project Structure > Project.

Em Project SDK, selecione o JDK 21.

Em Project language level, selecione 21 - (Java 21).

Certifique-se de que o Maven está configurado corretamente em Build, Execution, Deployment > Build Tools > Maven.
Reddit

📄 Licença
Este projeto está licenciado sob a Licença MIT. Consulte o arquivo LICENSE para obter mais informações.

Sinta-se à vontade para personalizar este README.md conforme as especificidades do seu projeto. Se precisar de mais alguma coisa, estou à disposição!
