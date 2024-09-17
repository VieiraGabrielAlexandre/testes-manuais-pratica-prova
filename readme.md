# Plano de Fluxo de Trabalho e Ciclo de Vida do Bug

## Introdução
Este documento descreve o fluxo de trabalho e o ciclo de vida do bug no processo de desenvolvimento de software, detalhando as etapas desde a identificação até a resolução final.

## Fluxo de Trabalho

### Identificação do Bug
Os bugs são identificados através de testes automatizados e feedback do usuário.

### Análise e Classificação
Prioridade é definida com base na gravidade e impacto no sistema.

### Atribuição
O bug é atribuído a um desenvolvedor responsável.

### Resolução
O desenvolvedor trabalha na correção do bug, com foco em garantir que a funcionalidade volte a operar normalmente.

### Teste e Validação
O time de QA realiza testes para garantir que a correção foi bem-sucedida e não causou outros problemas.

### Encerramento
O bug é marcado como resolvido e registrado no sistema de controle.

---

# User Stories

## User Story 1: Login de Usuário
**Título:** Login de Usuário

**Como** um usuário, **eu quero** fazer login com minhas credenciais **para** acessar minha conta e ver minhas informações personalizadas.

### Critérios de Aceitação:
1. O sistema deve permitir login com email e senha válidos.
2. Deve exibir uma mensagem de erro para credenciais inválidas.

## User Story 2: Recuperação de Senha
**Título:** Recuperação de Senha

**Como** um usuário, **eu quero** poder recuperar minha senha **para** redefinir meu acesso caso eu a perca.

### Critérios de Aceitação:
1. O sistema deve enviar um email com um link de redefinição.
2. O link deve expirar após 24 horas.

---

# Documentos de Teste

## a) Mind-map da User Story: Login de Usuário
Este é um mapa mental que descreve a User Story “Login de Usuário”, destacando os cenários e dependências.

## b) Casos de Teste Step-by-Step

### Caso de Teste 1: Testar Login com Credenciais Válidas
- **Título:** Testar Login com Credenciais Válidas
- **Objetivo:** Garantir que o sistema permite login com credenciais corretas.
- **Pré-condições:** O usuário deve estar registrado no sistema.
- **Passos:**
  1. Acessar a página de login.
  2. Inserir email e senha válidos.
  3. Clicar em “Entrar”.
- **Resultado Esperado:** O usuário deve ser redirecionado para o painel.

### Caso de Teste 2: Testar Login com Credenciais Inválidas
- **Título:** Testar Login com Credenciais Inválidas
- **Objetivo:** Garantir que o sistema exibe uma mensagem de erro para credenciais inválidas.
- **Pré-condições:** Nenhuma.
- **Passos:**
  1. Acessar a página de login.
  2. Inserir email ou senha inválidos.
  3. Clicar em “Entrar”.
- **Resultado Esperado:** O sistema deve exibir uma mensagem de erro.

## c) Casos de Teste BDD

### Caso de Teste 1: Login com Credenciais Válidas
- **Título:** Login com Credenciais Válidas
- **Cenário:**
  - **Dado que** o usuário está registrado no sistema,
  - **Quando** ele insere email e senha válidos,
  - **Então** ele deve ser redirecionado para o painel de usuário.

### Caso de Teste 2: Login com Credenciais Inválidas
- **Título:** Login com Credenciais Inválidas
- **Cenário:**
  - **Dado que** o usuário acessa a página de login,
  - **Quando** ele insere credenciais inválidas,
  - **Então** o sistema deve exibir uma mensagem de erro.
