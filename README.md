# 🦆 Linguados

Gamificação de idiomas através de desafios técnicos via CLI.

### Tecnologias
* **Linguagem:** Java 21 (JDK 21)
* **Gerenciamento de Dependências:** Maven
* **Banco de Dados:** MySQL 8.0
* **Infraestrutura:** Docker & Docker Compose
* **Automação:** GitHub Actions (CI/CD)

### Arquitetura do Projeto
O sistema segue o padrão **MVC (Model-View-Controller)**, organizado por módulos de domínio:

* `usuario/`: Gerenciamento de jogadores, login e autenticação.
* `desafio/`: Engine de desafios (Tradução, Lacuna e Múltipla Escolha).
* `progresso/`: Registro de atividades e histórico de resoluções.
* `conquista/`: Sistema de badges e recompensas por XP.
* `config/`: Configurações centrais e Singleton de conexão com BD.

### Como Rodar
1. Certifique-se de ter o **Docker** instalado.
2. Clone o repositório principal.
3. No terminal, execute:
   ```bash
   docker-compose up -d --build
   docker exec -it linguados-app java -jar app.jar
