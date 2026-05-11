# 🚀 Desafio 3 — Controle Financeiro

Bem-vindo ao terceiro desafio da Formação iOS.

Agora você irá evoluir do armazenamento em memória para um aplicativo com **persistência real de dados**, utilizando banco de dados local.

Este desafio marca a transição para um nível mais profissional de desenvolvimento iOS.

---

# 🎯 Objetivo do Desafio

Criar um aplicativo chamado **Controle Financeiro**, permitindo que o usuário:

- Registre receitas e despesas
- Visualize saldo atualizado
- Edite e exclua transações
- Filtre transações por tipo
- Visualize relatórios por categoria
- Armazene todos os dados localmente

⚠️ Importante:
Todos os dados devem ser persistidos no dispositivo utilizando banco de dados local.

---

# 🧠 Tecnologias que você irá praticar

Este desafio foi projetado para consolidar:

- Core Data
- Models / Entities
- Persistent Container
- Managed Object Context
- Fetch Requests
- NSPredicate
- NSSortDescriptor
- Migrations
- Relacionamentos (1-1, 1-N, N-N)
- Transformable Attributes
- CRUD completo

---

# 📱 Estrutura do Aplicativo

O aplicativo deve conter as seguintes telas:

1️⃣ Splash Screen  
2️⃣ Dashboard (Resumo Financeiro)  
3️⃣ Lista de Transações  
4️⃣ Cadastro / Edição de Transação  
5️⃣ Relatórios  

<img width="1158" height="595" alt="Captura de Tela 2026-02-25 às 21 01 21" src="https://github.com/user-attachments/assets/78f0abaf-f96f-4d3f-b1ec-f0cc4fb50cf2" />

---

# 🗂 Estrutura de Banco Esperada

## Entidades sugeridas

### Conta
- id
- nome

### Categoria
- id
- nome
- tipo (Receita ou Despesa)

### Transacao
- id
- descricao
- valor
- tipo
- data
- categoriaId
- contaId

---

# 🔗 Relacionamentos

- 1 Conta → N Transações
- 1 Categoria → N Transações
- Possível extensão futura para N-N (ex: Tags)

---

# 🔄 Migrações

Você deve:

- Criar pelo menos uma Migration
Exemplo:
- Adicionar campo “observacao” na transação
ou
- Adicionar campo “formaPagamento”

---

# 🧩 Regras Técnicas

- CRUD completo funcionando
- Uso de Core Data
- Estrutura organizada
- Banco isolado da camada de UI
- Uso de atributos compatíveis com persistência local
- Consultas usando `NSPredicate`
- Ordenação usando `NSSortDescriptor`


---

# ⭐ Parte Opcional (Avançado)
- Implementar histórico mensal
- Criar exportação simples em JSON
- Implementar múltiplas contas

---

# 🏁 Resultado Esperado

Ao concluir este desafio você será capaz de:

- Trabalhar com banco de dados local no iOS
- Estruturar Models / Entities corretamente
- Criar uma camada de persistência profissional
- Implementar relacionamentos
- Realizar consultas complexas
- Aplicar Migrations
- Desenvolver um app com persistência real
