# Visão Geral dos Microfrontends

O projeto é composto pelos seguintes microfrontends:

## tc2-mfe-shell
Aplicação container responsável por orquestrar e integrar os demais MFEs.

## tc2-mfe-main
Microfrontend principal que contém as funcionalidades centrais do sistema.

## tc2-mfe-auth
Microfrontend responsável pelos fluxos de autenticação e gerenciamento de sessão.

> [INFO!]
> Cada microfrontend possui responsabilidades bem definidas, evitando sobreposição de lógica.