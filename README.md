<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=header&text=Luis%20Fernando&fontSize=52&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Backend%20Engineer%20%E2%80%A2%20Java%20%E2%80%A2%20Spring%20Boot%20%E2%80%A2%20Kafka&descAlignY=60&descSize=18" alt="Luis Fernando — Backend Engineer" />

<a href="https://github.com/nando-sout"><img src="https://img.shields.io/badge/GitHub-nando--sout-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
<img src="https://img.shields.io/badge/Foco-Backend-2c5364?style=for-the-badge" alt="Foco: Backend" />
<img src="https://img.shields.io/github/followers/nando-sout?style=for-the-badge&logo=github&label=Seguidores" alt="Seguidores" />

</div>

---

## 👋 Olá, eu sou o Luis

Vim do **recrutamento técnico** e hoje construo minha carreira em **engenharia de software backend**. Ter visto de perto o que os times de tecnologia procuram me faz escrever código pensando em quem vai ler, testar e manter.

- 🔭 Construindo sistemas com **Java, Spring Boot, PostgreSQL e Kafka**
- 🧱 Gosto de arquitetura orientada a eventos, APIs bem documentadas e testes
- 💬 Pergunte-me sobre backend, recrutamento técnico ou transição de carreira

---

## 🛠️ Stack

<div align="center">

<img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" />
<img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" alt="Spring Boot" />
<img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white" alt="Spring Security" />
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
<img src="https://img.shields.io/badge/Apache%20Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white" alt="Kafka" />
<img src="https://img.shields.io/badge/Flyway-CC0200?style=for-the-badge&logo=flyway&logoColor=white" alt="Flyway" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
<img src="https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white" alt="Maven" />
<img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black" alt="Swagger" />
<br />
<img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React" />
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
<img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite" />
<img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git" />

</div>

---

## 🚀 Projetos em destaque

### 🛡️ [fraud-monitoring-api](https://github.com/nando-sout/fraud-monitoring-api)

API que registra transações financeiras e classifica o risco de fraude **sem travar quem está pagando**: a transação é gravada na hora e a análise acontece de forma assíncrona.

- **Outbox Pattern:** a transação e o evento são gravados na mesma transação de banco, e um publisher envia ao Kafka
- **Regras de fraude:** localização, valor e frequência de transações
- **Infra:** Kafka em modo KRaft, PostgreSQL 16, migrations com Flyway, tudo subindo com Docker Compose
- **Documentação:** 14 documentos técnicos cobrindo arquitetura, trade-offs, testes e segurança

```mermaid
flowchart LR
    A["POST /transactions"] --> B[("PostgreSQL<br/>Transaction + Outbox")]
    B --> C["OutboxPublisher"]
    C --> D{{"Kafka"}}
    D --> E["Consumer"]
    E --> F["Análise de fraude<br/>local · valor · frequência"]
    F --> B
```

`Java 25` `Spring Boot` `Kafka` `PostgreSQL` `Flyway` `Docker` `OpenAPI`

---

### 📊 Recruiter Visual

Ferramenta para recruiters acompanharem **vagas, etapas e candidatos de forma visual**, com funil e Kanban. Nasceu da minha experiência com recrutamento: o foco é enxergar e movimentar candidatos, não ser um ATS completo.

| | Repositório | O que tem |
|---|---|---|
| 🎨 | [**recruiter-visual**](https://github.com/nando-sout/recruiter-visual) | Interface em React 19 e TypeScript, com funil da vaga, Kanban e gráficos |
| ⚙️ | [**recruiter-visual-api**](https://github.com/nando-sout/recruiter-visual-api) | API em Spring Boot com login JWT, verificação de e-mail, etapas configuráveis, avaliação por etapa e histórico de auditoria |

**Destaques da API:** cada recruiter só acessa as próprias vagas, senhas e códigos são guardados com hash, e a taxa de reprovação é calculada por etapa.

`React 19` `TypeScript` `Vite` `Tailwind CSS` `Spring Boot` `Spring Security` `JWT` `PostgreSQL`

---

## 🌱 Outros repositórios

| Repositório | Situação |
|---|---|
| [vollMed](https://github.com/nando-sout/vollMed) | Projeto de estudo com Spring Boot, em construção |
| [LuisFernando_TechRecruiter](https://github.com/nando-sout/LuisFernando_TechRecruiter) | Repositório de 2023, com o README inicial |

---

## 📊 Estatísticas

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=nando-sout&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="Estatísticas do GitHub" />
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=nando-sout&layout=compact&theme=tokyonight&hide_border=true" alt="Linguagens mais usadas" />

</div>

---

<div align="center">

<sub>Feito com ☕ e Java</sub>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,100:0f2027&height=100&section=footer" alt="" />

</div>
