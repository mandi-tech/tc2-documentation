# Module Federation

O projeto utiliza **Webpack Module Federation** para permitir a integração de múltiplos microfrontends em tempo de execução.

## Como funciona

- O Shell declara os microfrontends como `remotes`
- Cada MFE expõe seus módulos publicamente
- O carregamento ocorre dinamicamente em runtime

## Vantagens

- Deploy independente
- Redução de dependências diretas
- Melhor isolamento de responsabilidades
