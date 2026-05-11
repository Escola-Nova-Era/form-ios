# 🚀 Desafio 5 — Tech Events (MVVM do Zero)

Bem-vindo ao quinto desafio da Formação iOS.

Neste desafio você vai criar um aplicativo **do zero**, aplicando **arquitetura MVVM** como uma aplicação profissional é construída no dia a dia.

O foco aqui é: organização, separação de responsabilidades e código escalável.

---

# 🎯 Objetivo do Desafio

Criar um aplicativo chamado **Tech Events** que:

- Consome uma API de eventos de tecnologia e programação
- Exibe uma lista paginada de eventos
- Permite buscar e filtrar eventos
- Exibe detalhe do evento
- (Opcional) permite criar/editar evento
- Implementa **MVVM** com **Repository Pattern**
- Modela estados de UI com **Enum com Associated Values**

⚠️ Importante:
- Este desafio **não usa DI**.
- O app deve ser criado **do zero** já em MVVM.

---

# 🌐 API Utilizada

Tech Events API (Mock)

Endpoints:

- `GET /events?page=1&limit=10`
- `GET /events/{id}`
- `POST /events`
- `PUT /events/{id}`
- `DELETE /events/{id}`

---

# 🧠 Tecnologias e Conceitos Trabalhados

## Arquitetura e iOS

- MVVM
- ViewModel
- UIKit
- UIViewController
- Closures para comunicação entre ViewModel e ViewController
- Combine ou async/await para atualização de estado
- Auto Layout

## Organização e Boas Práticas

- Repository Pattern
- Separação clara entre UI e dados
- Modelagem de estado de tela
- Extensions em Swift

## Conceitos Avançados

- Enum vs Struct
- Enum com Associated Values aplicado à arquitetura (UI State)
- Generics
- Protocols
- Type constraints em tipos genéricos

---

# 📱 Telas do Aplicativo

O aplicativo deve conter:

1️⃣ Splash  
2️⃣ Lista de Eventos (com busca e filtros)  
3️⃣ Detalhe do Evento  

<img width="1208" height="807" alt="Captura de Tela 2026-02-27 às 13 25 36" src="https://github.com/user-attachments/assets/b76caf7c-e68a-4e17-a244-5602a723d266" />


---

# 🏗 Estrutura Recomendada do Projeto

Uma estrutura simples e profissional (sem Clean completo ainda):
data/
api/
dto/
repository/

domain/
model/
repository/

presentation/
ui/
viewmodel/


✅ Observação:
- Você pode manter `domain` simples (somente models + interface do repository).
- A evolução para UseCases/Clean pode vir depois.

---

# 🔄 Estados de UI (Obrigatório)

Você deve modelar o estado da tela usando **Enum com Associated Values**.

Exemplo:

```swift
enum UiState<T> {
    case loading
    case success(T)
    case error(String)
    case empty
}
