# Erros Comuns

Este documento lista os problemas mais comuns encontrados durante o desenvolvimento local dos microfrontends do projeto **Tech Challenge – Fase 2**, bem como possíveis causas e soluções.

---

## 🚫 Porta já em uso

### Sintoma
Ao executar `ng serve`, a aplicação não inicia e retorna erro informando que a porta já está em uso.

### Causa
Outro processo (geralmente outro microfrontend) já está utilizando a mesma porta.

### Solução
- Verifique quais aplicações estão rodando localmente
- Encerre o processo que está utilizando a porta
- Ou execute a aplicação em outra porta:

```bash
ng serve --port 4300
```

---

## ⚠️ Versão incompatível do Node.js

### Sintoma
Erros inesperados durante instalação de dependências ou execução do projeto.

### Causa
Versão do Node.js diferente da utilizada no projeto.

### Solução
- Verifique a versão instalada:

```bash
node -v
```

- Utilize a versão recomendada (ver docs/setup/prerequisites.md)
- Recomenda-se o uso de nvm para gerenciar versões do Node

---

## 🔄 Dependências desalinhadas

### Sintoma
Erros de build, comportamento inconsistente ou falhas ao carregar microfrontends.

### Causa
Versões diferentes de dependências compartilhadas entre os MFEs.

### Solução
- Verifique se as versões de Angular e RxJS estão alinhadas
- Reinstale dependências:

```bash
rm -rf node_modules package-lock.json
npm install
```

- Confirme as configurações de dependências compartilhadas no Module Federation
