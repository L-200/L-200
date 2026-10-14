<div align="center">

# Olá, eu sou o Lucas! 👋

**Estudante de Ciência da Computação na UFAM · Desenvolvedor em formação**

_Em busca de me tornar um excelente programador, uma linha de código por vez._

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0077B5?style=for-the-badge&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/lucas-pereira-5629bb318/)
[![Gmail](https://img.shields.io/badge/-Gmail-D14836?style=for-the-badge&logo=Gmail&logoColor=white)](mailto:lucasscpereira14@gmail.com)

![UFAM](https://img.shields.io/badge/UFAM-Ci%C3%AAncia%20da%20Computa%C3%A7%C3%A3o-blue?style=flat-square)

</div>

---

## 👤 Sobre mim

Sou estudante de Ciência da Computação na **UFAM**, construindo minha base em desenvolvimento back end, bancos de dados, sistemas operacionais e engenharia de software. Gosto de projetos que unem teoria e prática: do escalonamento de threads a APIs REST e agentes baseados em LLM.

- 🎓 Cursando Ciência da Computação (UFAM)
- 🔭 Foco atual: **back end, APIs REST e bancos de dados**
- 🌱 Aprendendo e praticando: **Node.js, Express, MongoDB, Mongoose, Docker e LLMs locais**
- 🌌 Apaixonado pelo universo de **Star Wars**
- 🎮 Jogo favorito: **Hollow Knight**, pela trilha sonora, arte e complexidade do gameplay

---

## 🚀 Projetos em destaque

### 🃏 Nota Secreta: Agente Estratégico LLM

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![LLM](https://img.shields.io/badge/LLM-Phi--3.5--mini-8A2BE2)
![GGUF](https://img.shields.io/badge/modelo-GGUF%20Q4__K__M-orange)
![Trabalho em grupo](https://img.shields.io/badge/trabalho-em%20grupo-lightgrey)

Agente autônomo para o jogo **Nota Secreta** (uma variação de Dixit com músicas brasileiras), integrando um modelo de linguagem local (**Phi-3.5-mini-instruct**) a rotinas de _fallback_ heurístico em camadas, para garantir resiliência em um ambiente multiagente.

- **Arquitetura híbrida defensiva:** cada decisão combina chamada à LLM com camadas de fallback algorítmico (planos A/B/C), então o agente nunca trava a partida nem devolve resposta inválida
- **Engenharia de prompts:** few-shot, tentativas com temperaturas diferentes, saída em JSON estrito e índices posicionais para reduzir alucinações
- **Observabilidade:** logs separados por `run_id`, com `render_log_readable.py` para visualizar partidas e `analyze_decisions.py` para medir a taxa de sucesso da LLM versus cada fallback

### 🌐 Microsserviços: Back End Development and APIs

![Node.js](https://img.shields.io/badge/Node.js-6DA55F?logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-404d59?logo=express&logoColor=61DAFB)
![MongoDB](https://img.shields.io/badge/MongoDB-4ea94b?logo=mongodb&logoColor=white)
![Mongoose](https://img.shields.io/badge/Mongoose-880000?logo=mongoose&logoColor=white)
![Multer](https://img.shields.io/badge/Multer-upload-lightgrey)

Cinco microsserviços Node.js autônomos, desenvolvidos na certificação do freeCodeCamp: **Timestamp**, **Request Header Parser**, **URL Shortener**, **Exercise Tracker** e **File Metadata**.

- **APIs REST** com rotas, métodos HTTP, status codes (incluindo redirecionamento `302`) e respostas JSON consistentes
- **Persistência** com MongoDB e Mongoose, modelando usuários e exercícios relacionados
- **Consultas com filtros** por intervalo de datas (`from`, `to`) e limite de resultados (`limit`)
- **Validação de URLs** com consulta DNS ativa (`dns.lookup`) antes de gravar
- **Upload de arquivos** com Multer (`memoryStorage`), além de **Dotenv** e **CORS**

### ☕ Ryusei Café: Sistema de Gerenciamento

![Java](https://img.shields.io/badge/Java-17%2B-ED8B00?logo=openjdk&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?logo=apachemaven&logoColor=white)
![Swing](https://img.shields.io/badge/GUI-Swing-blue)

Projeto final de **POO**: sistema de gestão de um Manga Café com interface gráfica (Swing) e modo CLI, evoluindo de persistência em memória para integração com **PostgreSQL**.

- **Padrão DAO** separando lógica de negócio e acesso ao banco, com **JDBC** e _Prepared Statements_
- **Interfaces e polimorfismo** (`Vendivel`) e **herança** (`Pessoa` → `Funcionario` / `Usuario`) refletida no modelo relacional
- Vendas com carrinho e baixa de estoque transacional, CRUD de clientes e funcionários e criação automática das tabelas via `init.sql`

### 🖥️ Trabalhos Práticos de Sistemas Operacionais I

![C](https://img.shields.io/badge/C-A8B9CC?logo=c&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)

- **TP1:** escalonamento e concorrência, com cenários de _race conditions_ (leitores × escritores, produtores × consumidores) resolvidos com **semáforos**
- **TP2:** ganho de desempenho com **threads** em multiplicação matricial, produto escalar e simulação de servidor web, com relatório e gráficos gerados em Python

### 🗄️ Bancos de Dados

| Projeto                                                                                                          | Descrição                                                                                                                                                                                                       | Tecnologias                                                                                                                                                                                                                                                       |
| ---------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Trabalho Prático 1: ETL Amazon                        | Pipeline **ETL** que processa o dataset de produtos da Amazon (SNAP) e carrega em PostgreSQL com esquema projetado _bottom-up_ e normalizado até a **4FN**, mais um dashboard de consultas                      | ![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white) |
| Trabalho Prático 2: Armazenamento em memória secundária| Programas em **C++17** para armazenar e consultar artigos científicos em disco, com arquivo de dados em **Hashing** (endereçamento aberto) e índices em **Árvore B+** (primário por ID e secundário por título) | ![C++](https://img.shields.io/badge/C++17-00599C?logo=cplusplus&logoColor=white) ![Make](https://img.shields.io/badge/GNU%20Make-lightgrey) ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)                                     |

---

## 🧠 Principais conhecimentos

### Linguagens

<p>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/c/c-original.svg" height="40" alt="C" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/cplusplus/cplusplus-original.svg" height="40" alt="C++" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" height="40" alt="Python" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original.svg" height="40" alt="Java" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg" height="40" alt="JavaScript" />
</p>

### Back end e bancos de dados

<p>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nodejs/nodejs-original.svg" height="40" alt="Node.js" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mongodb/mongodb-original.svg" height="40" alt="MongoDB" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/postgresql/postgresql-original.svg" height="40" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Mongoose-880000?logo=mongoose&logoColor=white" height="28" alt="Mongoose" />
</p>

### Ferramentas

<p>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/docker/docker-original.svg" height="40" alt="Docker" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/maven/maven-original.svg" height="40" alt="Maven" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/npm/npm-original-wordmark.svg" height="40" alt="npm" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/git/git-original.svg" height="40" alt="Git" />
</p>

<details>
<summary><b>Resumo em tabela</b></summary>

| Área            | Tecnologias e conceitos                                                                |
| --------------- | -------------------------------------------------------------------------------------- |
| Linguagens      | C, C++17, Python, Java 17, JavaScript                                                  |
| Back end        | Node.js, Express, Multer, CORS, Dotenv, JDBC, APIs REST                                |
| Bancos de dados | PostgreSQL, MongoDB, Mongoose, ETL, normalização (4FN), Hashing, Árvore B+             |
| IA              | LLM local (Phi-3.5, GGUF), engenharia de prompts, fallback heurístico, análise de logs |
| Sistemas        | Threads, semáforos, escalonamento, race conditions                                     |
| Engenharia      | POO, padrão DAO, polimorfismo, Docker e Docker Compose, Maven, GNU Make, Git LFS       |

</details>

---

> _"Aprender é a única coisa que a mente nunca se cansa, nunca tem medo e nunca se arrepende"_, Leonardo da Vinci
