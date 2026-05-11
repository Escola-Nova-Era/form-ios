# 🚀 Desafio 2 — Aplicativo de Eventos

Bem-vindo ao segundo desafio da Formação iOS.

Agora você irá evoluir do mundo das telas simples para trabalhar com **listas dinâmicas**, manipulação de dados em memória e organização de informações em tempo real.

Este desafio consolida sua base em UI e introduz estruturas fundamentais para qualquer app moderno.

---

# 🎯 Objetivo do Desafio

Criar um aplicativo chamado **Eventos**, contendo:

- Splash Screen
- Tela principal com lista de eventos
- Funcionalidade de busca
- Funcionalidade de ordenação
- Atualização dinâmica da lista
- Navegação para tela de detalhe do evento

⚠️ Importante:
- Não utilizar API
- Não utilizar banco de dados
- Todos os dados devem estar em memória

---

# 🧠 Tecnologias que você irá praticar

Este desafio foi projetado para consolidar os seguintes conceitos:

- UITableView
- UITableViewDataSource
- UITableViewDelegate
- UITableViewCell
- UICollectionView
- UICollectionViewDataSource
- UICollectionViewDelegate
- UICollectionViewFlowLayout
- UIStackView
- UISearchBar
- UISearchController
- Atualização dinâmica de listas
- Swift Collections (Array, Set, Dictionary)
- Closures
- Funções de alta ordem
- Structs
- Manipulação de dados dinâmicos

---

# 📱 Estrutura do Aplicativo

O aplicativo deve conter 3 partes principais.

<img width="796" height="763" alt="Captura de Tela 2026-02-25 às 18 50 38" src="https://github.com/user-attachments/assets/c2c97769-1f73-4fd6-bae7-4112bc59620a" />


---

# 🟢 Tela 1 — Splash Screen

Objetivo:
Apresentar o aplicativo ao usuário.

Elementos esperados:

- Ícone central
- Nome do app: “Eventos”
- Subtítulo
- Versão do aplicativo
- Layout minimalista

Tecnologias aplicadas:
- UIViewController
- Organização de layout
- Auto Layout
- Temas, cores e estilos

---

# 🟡 Tela 2 — Lista de Eventos

Objetivo:
Exibir eventos dinamicamente utilizando UITableView ou UICollectionView.

## 🔹 Estrutura visual

Cada item deve conter:

- Categoria (label, badge ou componente customizado)
- Nome do evento
- Data e hora
- Local
- Indicador visual (ex: Hoje / Esta semana)
- Ícone de navegação

Utilizar:
- UITableViewCell ou UICollectionViewCell
- Auto Layout
- UIStackView
- Layout vertical

---

# 🔎 Funcionalidade de Busca

Criar campo de busca que:

- Filtre eventos pelo nome
- Filtre por categoria
- Atualize a lista dinamicamente

Aplicar:
- `filter`
- Closures
- Atualização da UITableView ou UICollectionView

---

# ↕ Funcionalidade de Ordenação

Permitir ordenar por:

- Nome (A-Z)
- Data (mais próxima)
- Categoria

Aplicar:
- `sorted`
- `sorted(by:)`
- Manipulação da lista original

---

## 🧩 Regras Técnicas

- Lista inicial com no mínimo 6 eventos mockados  
- A lista deve ser mutável  
- Utilizar boas práticas no DataSource e Delegate  
- Código organizado  
- Separação clara de responsabilidades  

---

## ⭐ Parte Opcional (Avançado)

- Implementar agrupamento por categoria  
- Implementar contagem dinâmica de eventos  
- Implementar estado vazio (Nenhum evento encontrado)  
- Criar versão alternativa usando UICollectionView  

---

## 🏁 Resultado Esperado

Ao concluir este desafio você será capaz de:

- Criar listas dinâmicas com UITableView ou UICollectionView  
- Criar e organizar células customizadas  
- Manipular coleções Swift  
- Filtrar e ordenar dados    

Você agora domina a base de qualquer aplicativo moderno baseado em listas.
