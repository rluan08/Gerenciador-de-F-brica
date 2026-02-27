Factory Manager
O Factory Manager PRO é um sistema de gestão industrial focado no controle de matérias-primas, gerenciamento de catálogo de produtos e otimização de produção. O sistema utiliza algoritmos para sugerir a melhor ordem de fabricação baseando-se no estoque disponível para maximizar o retorno financeiro.
Funcionalidades
• Gestão de Inventário: Cadastro, edição e exclusão de matérias-primas com controle de saldo em tempo real.
• Catálogo de Produtos: Cadastro de produtos com definição de receitas (composição detalhada) e preços de venda.
• Otimização de Produção: Algoritmo inteligente que calcula a sugestão de produção ideal para obter o maior lucro possível com os recursos atuais em estoque.
• Internacionalização (i18n): Interface com suporte dinâmico para múltiplos idiomas, incluindo Português (BR) e Inglês (US).
• Interface Moderna: Painel responsivo construído com as melhores práticas de UI/UX utilizando Vue 3 e CSS avançado.
Tecnologias Utilizadas
Back-end
• Java 17
• Spring Boot 3
• Spring Data JPA
• H2 Database (Banco de dados em memória, ideal para desenvolvimento e testes rápidos)
Front-end
• Vue.js 3 (Composition API)
• Axios (Integração assíncrona com a API)
• Vue i18n (Gerenciamento de internacionalização e localização)
• Vite (Ferramenta de build rápida para o front-end)
Como rodar o projeto
Este projeto é dividido em duas partes: Back-end (API) e Front-end (Interface). Para que o sistema funcione corretamente, você deve manter dois terminais abertos simultaneamente (um para cada parte).
Você pode utilizar qualquer terminal de sua preferência (CMD, PowerShell, Bash, Terminal do Linux/Mac) ou os terminais integrados de editores como VS Code e IntelliJ.
1. Pré-requisitos
• Navegador Web Instalado 
• Java 17 ou superior instalado.
java -version
• Node.js e npm instalado.
node -v
npm -v
2. Passo 1: Rodando o Back-end (API)
Abra o primeiro terminal na pasta raiz do projeto back-end e digite :
mvnw.cmd spring-boot:run

Rodar No Linux ou Mac (Bash/Zsh):
./mvnw spring-boot:run

Nota: O servidor iniciará em http://localhost:8082. Não feche este terminal enquanto estiver usando o sistema.

3. Passo 2: Rodando o Front-end (Interface)
Abra um novo terminal (separado do primeiro) na pasta do front-end:

Entre na pasta do front-end
cd factory-frontend

Instale as dependências (necessário apenas na primeira vez)
npm install

Inicie o servidor de desenvolvimento
npm run dev

Nota: O terminal informará um link (geralmente http://localhost:5173). Copie e cole no seu navegador para acessar o sistema.

Dicas de Execução
• Ambiente Multiplataforma: O projeto foi configurado para rodar nativamente em Windows, Linux e macOS através dos wrappers do Maven.
• Terminais Independentes: Lembre-se que o Back-end e o Front-end são processos separados. Se um deles for fechado, o sistema perderá a conexão.
• Banco de Dados: O sistema utiliza o banco de dados H2 em memória. Isso significa que, ao reiniciar o terminal do Back-end, os dados serão resetados para o estado inicial.
Estrutura de Internacionalização (i18n)
A tradução do sistema é gerenciada via arquivos JSON localizados em src/locales/. A troca de idioma ocorre em tempo real no componente principal através de chaves dinâmicas, garantindo uma aplicação escalável para novos mercados.

Autor

Luan dos Santos Ribeiro

Estudante de Engenharia de Computação e desenvolvedor focado em soluções para automação, otimização e sistemas de apoio à decisão.
