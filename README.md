# Tech Challenge – Fase 2 | Documentação

Este repositório centraliza toda a **documentação técnica e funcional** do projeto **Tech Challenge – Fase 2**, que utiliza uma arquitetura baseada em **Microfrontends**.

Aqui estão descritos os conceitos de arquitetura, padrões adotados, guias de setup, convenções de código e documentação específica de cada microfrontend.

<br />

## 📦 Repositórios do Projeto

O projeto é composto pelos seguintes repositórios:

- **tc2-mfe-shell** → Aplicação container (Shell/Host)
- **tc2-mfe-main** → Microfrontend principal da aplicação
- **tc2-mfe-auth** → Microfrontend de autenticação
- **tc2-documentation** → Documentação central (este repositório)
- **backend-tech-challenge-2** → API disponibilizada pela FIAP

<br />

## 🧱 Arquitetura

A aplicação segue o padrão **Microfrontends com Module Federation**, onde:

- O **Shell** é responsável por orquestrar os MFEs
- Os microfrontends são carregados dinamicamente
- Cada MFE é independente em build, deploy e versionamento
- Existe baixo acoplamento entre os módulos

Mais detalhes em:
📄 `docs/architecture/overview.md`

<br />

## 🎨 Design System

Para garantir consistência visual e reutilização de componentes entre os microfrontends, o projeto utiliza um **Design System centralizado**, documentado e mantido no GitBook.

Essa documentação contempla:
- Identidade visual
- Componentes reutilizáveis
- Tokens de design
- Boas práticas de uso entre MFEs

🔗 Acesse o Design System no GitBook: https://mandi-tech.gitbook.io/design-system-tc2

<br />

## 📂 Estrutura da Documentação

```
docs/
├── architecture/ # Visão geral e decisões arquiteturais
├── setup/ # Setup e execução local
├── microfrontends/ # Documentação específica de cada MFE
├── standards/ # Padrões e convenções
├── deployment/ # CI/CD e ambientes
└── troubleshooting/ # Problemas comuns
```

<br />

## 🚀 Como começar

Se você está entrando agora no projeto, siga esta ordem:

1. 📄 `docs/architecture/overview.md`
2. 📄 `docs/setup/environment-setup.md`
3. 📄 `docs/microfrontends/shell.md`

<br />

## 🤝 Contribuição

Este repositório é mantido como **fonte única da verdade** do projeto.  
Atualizações na arquitetura, padrões ou fluxos devem ser refletidas aqui.

<br />

## 📄 Licença

Projeto desenvolvido para o **Tech Challenge – Fase 2**.
