# 🚀 Desafio 4 — Characters App (Consumo de API + Paginação)

Bem-vindo ao quarto desafio da Formação iOS.

Agora você irá trabalhar com **consumo de API real**, controle de requisições assíncronas e paginação, utilizando boas práticas de rede no iOS.

Este desafio marca sua entrada no mundo de aplicações conectadas à internet.

---

# 🎯 Objetivo do Desafio

Criar um aplicativo chamado **Characters**, que:

- Consome uma API pública
- Lista personagens com paginação infinita
- Permite buscar personagens por nome
- Exibe detalhes de um personagem
- Permite favoritar personagens (armazenamento local com Core Data)

⚠️ Importante:
- Dados principais vêm da API
- Favoritos devem ser persistidos localmente com Core Data
- Não utilizar arquitetura avançada (MVVM vem no próximo nível)

---

# 🌐 API Utilizada

Rick and Morty API  
Base URL:
https://rickandmortyapi.com/api


Endpoints utilizados:

- `GET /character` → Lista com paginação
- `GET /character/{id}` → Detalhe do personagem

---

# 🧠 Tecnologias que você irá praticar

Este desafio consolida:

- URLSession
- async/await
- DispatchQueue
- Requisições GET
- Paginação
- URLRequest
- Tratamento de erro
- Estados de loading
- Core Data (para favoritos)

---

# 📱 Estrutura do Aplicativo

O app deve conter 3 telas principais:

1️⃣ Splash  
2️⃣ Lista de Personagens  
3️⃣ Detalhe do Personagem  

<img width="1186" height="796" alt="Captura de Tela 2026-02-27 às 12 46 12" src="https://github.com/user-attachments/assets/8fb78dc7-d894-4c33-b087-0a92587dc5c2" />


---

# 🟢 Tela 1 — Splash

- Nome do app
- Ícone central
- Layout minimalista
- Transição automática para lista

---

# 🟡 Tela 2 — Lista de Personagens

Deve conter:

- NavigationBar
- Campo de busca
- UITableView ou UICollectionView com células customizadas
- Scroll infinito (paginação)
- Loader no final da lista
- Estado de erro
- Estado vazio

Cada item deve exibir:

- Imagem do personagem
- Nome
- Status (Alive, Dead, Unknown)
- Espécie
- Ícone de favorito ⭐

Funcionalidades:

- Buscar por nome
- Carregar próxima página automaticamente
- Favoritar personagem (Core Data)

---

# 🔵 Tela 3 — Detalhe do Personagem

Deve exibir:

- Imagem grande
- Nome
- Status
- Espécie
- Gênero
- Origem
- Localização atual
- Botão para favoritar

---

# ⭐ Favoritos (Core Data)

Os favoritos devem ser persistidos localmente.

Você deve:

- Criar uma Entity
- Criar um Persistent Container
- Criar operações de busca, inserção, atualização e remoção
- Implementar CRUD básico para favoritos

Exemplo de Model:

```swift
struct FavoriteCharacter {
    let id: Int
    let name: String
    let image: String
    let status: String
}
