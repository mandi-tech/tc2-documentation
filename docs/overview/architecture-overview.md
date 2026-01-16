# Visão Geral da Arquitetura

A arquitetura do projeto segue o padrão de **Microfrontends**, onde cada aplicação frontend é construída, versionada e implantada de forma independente.

## Componentes Principais

- **Shell (Host)**: aplicação container responsável pela orquestração
- **Microfrontends Remotos**: aplicações independentes carregadas dinamicamente

## Benefícios da Arquitetura

- Baixo acoplamento entre módulos
- Deploy independente
- Escalabilidade do time
- Evolução tecnológica gradual

## Integração

A integração entre os microfrontends ocorre por meio do **Module Federation**, permitindo carregamento remoto em runtime.
