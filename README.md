# Factory Manager PRO

O Factory Manager PRO é um sistema de gestão industrial focado no controle de matérias-primas, gerenciamento de catálogo de produtos e otimização de produção. O sistema utiliza algoritmos para sugerir a melhor ordem de fabricação baseando-se no estoque disponível para maximizar o retorno financeiro.

---

## Funcionalidades

- Gestão de Inventário: cadastro, edição e exclusão de matérias-primas com controle de saldo em tempo real.  
- Catálogo de Produtos: cadastro de produtos com definição de receitas (composição detalhada) e preços de venda.  
- Otimização de Produção: algoritmo que calcula a sugestão de produção ideal para obter o maior lucro possível com os recursos disponíveis em estoque.  
- Internacionalização (i18n): interface com suporte dinâmico para múltiplos idiomas, incluindo Português (BR) e Inglês (US).  
- Interface Moderna: painel responsivo construído com Vue 3 e CSS avançado.  

---

## Tecnologias Utilizadas

### Back-end

- Java 17  
- Spring Boot 3  
- Spring Data JPA  
- H2 Database (banco em memória para desenvolvimento e testes)

### Front-end

- Vue.js 3 (Composition API)  
- Axios (integração com a API)  
- Vue i18n (internacionalização)  
- Vite (build e servidor de desenvolvimento)

---

## Como rodar o projeto

O projeto é dividido em duas partes: Back-end (API) e Front-end (Interface).  
Para funcionamento correto, mantenha dois terminais abertos simultaneamente.

Você pode utilizar qualquer terminal (CMD, PowerShell, Bash, Terminal Linux/Mac) ou terminal integrado de IDE.

---

### 1. Pré-requisitos

- Navegador web instalado  
- Java 17 ou superior

```bash
java -version
```

- Node.js e npm

```bash
node -v
npm -v
```

---

### 2. Rodando o Back-end (API)

Abra um terminal na pasta do back-end e execute:

**Windows**

```bash
mvnw.cmd spring-boot:run
```

**Linux / Mac**

```bash
./mvnw spring-boot:run
```

O servidor iniciará em:

```
http://localhost:8082
```

Não feche este terminal enquanto estiver utilizando o sistema.

---

### 3. Rodando o Front-end (Interface)

Abra um novo terminal na pasta do front-end:

```bash
cd factory-frontend
npm install
npm run dev
```

O terminal exibirá um link (geralmente):

```
http://localhost:5173
```

Acesse pelo navegador.

---

## Dicas de execução

- Ambiente multiplataforma: o projeto roda em Windows, Linux e macOS através do Maven Wrapper.  
- Processos independentes: Back-end e Front-end são processos separados. Se um for encerrado, a aplicação perde a comunicação.  
- Banco de dados: o H2 é em memória. Ao reiniciar o Back-end, os dados são resetados.  

---

## Estrutura de Internacionalização (i18n)

As traduções estão em arquivos JSON dentro de `src/locales/`.  
A troca de idioma ocorre dinamicamente no componente principal por meio de chaves, permitindo escalabilidade para novos idiomas.

---

## Autor

Luan dos Santos Ribeiro

Estudante de Engenharia de Computação e desenvolvedor focado em soluções para automação, otimização e sistemas de apoio à decisão.
