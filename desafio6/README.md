# 🚀 Desafio 6 — Pokédex com Testes Profissionais

Bem-vindo ao sexto desafio da Formação iOS.

Agora você não vai apenas criar um aplicativo funcional.

Você vai provar que ele funciona.

Este desafio é focado em **testes profissionais**, qualidade de código e cobertura.

---

# 🎯 Objetivo do Desafio

Criar um aplicativo chamado **Pokédex**, que:

- Consome a PokéAPI
- Lista Pokémons com paginação
- Permite buscar por nome
- Exibe detalhe do Pokémon
- Implementa testes unitários e testes de UI
- Alcança cobertura mínima de código

---

# 🌐 API Utilizada

PokéAPI

Base URL:
https://pokeapi.co/api/v2/


Endpoints utilizados:

- `GET /pokemon?limit=20&offset=0`
- `GET /pokemon/{id}`
- `GET /pokemon/{name}`

---

# 🧠 Tecnologias Obrigatórias

## 🔥 Testes

- Teste Unitário
- XCTest
- Test Doubles
- Mock
- Stub
- Fake
- Testes assíncronos
- XCUITest
- Coverage

---

# 📱 Estrutura do Aplicativo

O app deve conter:

1️⃣ Splash  
2️⃣ Lista de Pokémons  
3️⃣ Detalhe do Pokémon  

<img width="881" height="636" alt="Captura de Tela 2026-02-27 às 13 42 58" src="https://github.com/user-attachments/assets/bd12c155-598a-4f20-a17b-9dcda3f17bf4" />

---

# 🔄 Funcionalidades Obrigatórias

- Paginação (scroll infinito ou botão “carregar mais”)
- Busca por nome
- Estados de tela:
  - Loading
  - Success
  - Error
  - Empty

---

# 🧪 O que Deve Ser Testado

## ✅ Testes Unitários

- Mapeamento DTO → Model
- Formatação de número (#001)
- Conversão de altura e peso
- Funções utilitárias

---

## ✅ Testes de ViewModel

Utilizando:

- XCTest
- Test Doubles
- Mock
- Stub
- Fake

Você deve testar:

- Emissão de estado `Loading`
- Emissão de estado `Success`
- Emissão de estado `Error`
- Caso de lista vazia

---

## ✅ Testes de Repository

- Mock da API
- Simular erro de rede
- Simular retorno vazio

---

## ✅ Testes de UI (XCUITest)

Você deve testar:

- Lista aparece após loading
- Busca filtra corretamente
- Clique em item abre detalhe
- Tela de erro aparece quando API falha
- Botão “Tentar novamente” funciona

---

# 📊 Cobertura de Código (Coverage)

Meta mínima:

- 60% de cobertura

Meta recomendada:

- 70% ou mais

Cobrir principalmente:

- ViewModel
- Repository
- Funções de transformação

---

# 🧩 Regras Técnicas

- Não colocar lógica dentro da ViewController
- ViewModel deve expor estado observável
- Repository deve isolar API
- Testes não podem depender de internet real
- Usar dependências mockadas/fakes para testes assíncronos
- Não usar delays reais nos testes

---

# ⭐ Parte Opcional (Avançado)

- Implementar favoritos com Core Data e testar camada de persistência
- Implementar Retry automático
- Criar wrapper genérico `Result`
- Testar navegação com XCUITest
- Criar FakeRepository para testes

---

# 🏁 Resultado Esperado

Ao concluir este desafio você será capaz de:

- Escrever testes unitários reais
- Mockar dependências com Test Doubles
- Testar fluxos assíncronos corretamente
- Escrever testes de UI com XCUITest
- Medir cobertura de código
- Desenvolver aplicações mais seguras e confiáveis

Você agora está programando como alguém que trabalha em empresa.

No próximo desafio você irá evoluir esse conhecimento aplicando Injeção de Dependência.
