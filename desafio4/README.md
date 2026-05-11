# 🚀 Desafio 4 — Characters App (Consumo de API + Paginação)

Bem-vindo ao quarto desafio da Formação Android.

Agora você irá trabalhar com **consumo de API real**, controle de requisições assíncronas e paginação, utilizando boas práticas de rede no Android.

Este desafio marca sua entrada no mundo de aplicações conectadas à internet.

---

# 🎯 Objetivo do Desafio

Criar um aplicativo chamado **Characters**, que:

- Consome uma API pública
- Lista personagens com paginação infinita
- Permite buscar personagens por nome
- Exibe detalhes de um personagem
- Permite favoritar personagens (armazenamento local com Room)

⚠️ Importante:
- Dados principais vêm da API
- Favoritos devem ser persistidos localmente com Room
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

- Retrofit
- Coroutines
- Threads
- Requisições GET
- Paginação
- Interceptor
- Tratamento de erro
- Estados de loading
- Room Database (para favoritos)

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

- TopAppBar
- Campo de busca
- RecyclerView com CardView
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
- Favoritar personagem (Room)

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

# ⭐ Favoritos (Room Database)

Os favoritos devem ser persistidos localmente.

Você deve:

- Criar uma Entity
- Criar DAO
- Criar Database
- Implementar CRUD básico para favoritos

Exemplo de Entity:

```kotlin
@Entity
data class FavoriteCharacter(
    @PrimaryKey val id: Int,
    val name: String,
    val image: String,
    val status: String
)
```
## 🔄 Paginação

- Utilizar o campo `page` da API  
- Carregar próxima página ao atingir o fim da lista  
- Evitar múltiplas requisições simultâneas  
- Exibir loader no rodapé da lista  

---

## ❗ Tratamento de Erros

Você deve tratar:

- Sem conexão  
- Timeout  
- Erro 404 (busca sem resultado)  
- Erro 500  

Exibir:

- Tela de erro amigável  
- Botão “Tentar novamente”  

---

## 🧩 Regras Técnicas

- Uso obrigatório de Retrofit  
- Uso obrigatório de Coroutines  
- Interceptor configurado  
- Tratamento de erro adequado  
- Paginação funcional  
- Favoritos persistidos com Room  
- Código organizado  
- Separação clara entre camada de rede e UI  

---

## ⭐ Parte Opcional (Avançado)

- Filtro por status  
- Filtro por gênero  
- Tela exclusiva de favoritos  
- Skeleton loading  
- Cache simples de última busca  

---

## 🏁 Resultado Esperado

Ao concluir este desafio você será capaz de:

- Consumir APIs reais  
- Trabalhar com requisições assíncronas  
- Implementar paginação  
- Tratar erros de rede  
- Trabalhar com estados de loading  
- Persistir dados locais com Room  
- Criar aplicações conectadas de nível intermediário  

Você agora domina o fluxo completo de comunicação entre app e servidor.

No próximo nível você aprenderá a organizar isso usando arquitetura profissional (MVVM).
