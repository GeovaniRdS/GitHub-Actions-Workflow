# 🌐 GitHub Pages Deployment Workflow

[![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)](https://github.com/features/actions)
[![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-222222?style=for-the-badge&logo=github&logoColor=white)](https://pages.github.com/)

Este repositório demonstra a implementação de um pipeline de **CI/CD** automatizado utilizando GitHub Actions. O objetivo é realizar o deploy automático de um site estático sempre que houver alterações específicas no conteúdo.

## 🎯 Objetivo do Projeto
Aprender e aplicar os conceitos de integração e entrega contínua, garantindo que mudanças no arquivo `index.html` sejam validadas e publicadas automaticamente no GitHub Pages sem intervenção manual.

## ⚙️ Funcionalidades
- **Gatilho Inteligente:** O workflow só é disparado quando ocorrem mudanças no arquivo `index.html`.
- **Deploy Automatizado:** Publicação imediata para o ambiente de produção (GitHub Pages).
- **Branch Protection:** Foco no fluxo de trabalho da branch `main`.

## 🛠️ Tecnologias Utilizadas
- **HTML5:** Para a estrutura do site estático.
- **YAML:** Para a configuração do workflow do GitHub Actions.
- **GitHub Pages:** Como provedor de hospedagem estática.

## 🚀 Como este Workflow Funciona

O arquivo `.github/workflows/deploy.yml` está configurado para:
1. Escutar eventos de `push` na branch `main`.
2. Filtrar alterações no arquivo `index.html` via `paths`.
3. Utilizar as Actions oficiais `actions/checkout` e `actions/upload-pages-artifact`.

## 📂 Estrutura do Repositório
```text
.
├── .github/workflows/
│   └── deploy.yml      # Configuração do CI/CD
├── index.html          # Site estático principal
└── README.md           # Documentação do projeto
```

## 🎯 Contexto do Projeto
Este projeto foi desenvolvido como parte do caminho de aprendizado da [[roadmap.sh](https://roadmap.sh/devops/projects)](https://roadmap.sh/projects/github-actions-deployment-workflow), focado em desafios reais de **DevOps**. O objetivo é consolidar conhecimentos em automação de tarefas, manipulação de fluxos de dados no Linux e monitorização de recursos.
