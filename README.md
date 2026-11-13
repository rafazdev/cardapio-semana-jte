# 🍳 Cardápio da Semana — Spring Boot + JTE (Versão 2)

Aplicação web desenvolvida em **Java com Spring Boot** e **JTE (Java Template Engine)** para planejamento de refeições semanais, com armazenamento em memória (`List<Prato>`), menu lateral reaproveitado e controle de pratos planejados e feitos.

## 🚀 Funcionalidades Implementadas

- **Layout Reaproveitado (`layout.jte`):** Menu lateral fixo presente em todas as páginas.
- **Página Inicial (`GET /`):** Apresentação do sistema e cartões de estatísticas em tempo real (pratos planejados, pratos feitos e data do próximo prato).
- **Adicionar Prato (`GET /pratos/novo` e `POST /pratos`):** Formulário completo com binding automático para a classe `Prato` e painel lateral de pré-visualização em tempo real.
- **Meu Cardápio (`GET /pratos`):** Listagem dinâmica dos pratos planejados, tratamento de lista vazia e botão **"Fiz!"** para mover o prato para o histórico de concluídos.
- **Pratos Feitos (`GET /feitos`):** Histórico das refeições concluídas com sistema de avaliação de 1 a 5 estrelas.

## 🛠️ Tecnologias Utilizadas

- Java 17
- Spring Boot 3.3.5 (Spring Web)
- JTE 3.1.12 (Java Template Engine)
- HTML5, CSS3 e JavaScript puro (para o resumo dinâmico do formulário)

## ▶️ Como Executar o Projeto

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/cardapio-semana-jte.git
   cd cardapio-semana-jte
   ```

2. Execute a aplicação via Maven:
   ```bash
   ./mvnw spring-boot:run
   ```
   *(No Windows, utilize `mvnw.cmd spring-boot:run` ou execute a classe `CardapioApplication.java` pela sua IDE).*

3. Acesse no navegador:
   ```
   http://localhost:8080/
   ```
