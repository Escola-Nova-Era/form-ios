# 🚀 Desafio 1 — Simulador de Investimentos

Bem-vindo ao primeiro desafio da Formação iOS.

Neste desafio você irá construir um aplicativo completo chamado **Simulador de Investimentos**, colocando em prática os fundamentos essenciais do desenvolvimento iOS.

O objetivo aqui não é apenas fazer funcionar — é entender como as telas se comunicam, como o ciclo de vida funciona e como estruturar interfaces profissionais.

---

# 🎯 Objetivo do Desafio

Criar um aplicativo com múltiplas telas que:

- Recebe dados do usuário
- Realiza cálculos com base em juros compostos
- Navega entre telas
- Exibe o resultado de forma organizada
- Utiliza componentes reutilizáveis para modularizar a interface

---

# 🧠 Tecnologias que você irá praticar

Este desafio foi projetado para consolidar os seguintes conceitos:

- Swift
- UIKit
- UIViewController
- Navegação entre ViewControllers
- Ciclo de vida de ViewController
- Passagem de dados entre telas
- Passagem de objetos entre telas
- Storyboard ou ViewCode
- Auto Layout
- UIScrollView
- UITextField
- UIButton
- UILabel
- UIStackView
- Temas, cores e estilos
- Organização de views
- Componentização de interface

---

# 📱 Estrutura do Aplicativo

O aplicativo deve conter **3 telas principais**.

<img width="1203" height="790" alt="Captura de Tela 2026-02-25 às 18 29 18" src="https://github.com/user-attachments/assets/41143ddc-03f6-4767-9825-3de4f8728de4" />

---

## 🟢 Tela 1 — Boas-vindas

Objetivo:  
Apresentar o app ao usuário.

Elementos esperados:

- Ícone ilustrativo
- Título: “Simulador de Investimentos”
- Texto explicativo
- Botão: “Começar Simulação”

Ao clicar no botão:  
➡ Navegar para a tela de configuração.

Tecnologias aplicadas:

- UIViewController
- Navegação entre ViewControllers
- Temas, cores e estilos
- Organização de layout com Auto Layout
- UIButton
- UILabel
- UIImageView

---

## 🟡 Tela 2 — Configuração da Simulação

Objetivo:  
Coletar os dados do usuário.

Campos obrigatórios:

- Valor inicial
- Aporte mensal
- Taxa de juros (% ao ano)
- Tempo (anos)

Requisitos técnicos:

- Utilizar `UITextField`
- Organizar os campos dentro de uma `UIScrollView`
- Validar entradas
- Organizar a interface com `Auto Layout`
- Utilizar `UIStackView` para facilitar a distribuição dos elementos

Botão:  
➡ “Calcular Investimento”

Ao clicar:

- Realizar o cálculo
- Criar um objeto com os dados da simulação
- Passar os dados para o próximo `UIViewController`

Tecnologias aplicadas:

- Passagem de dados entre ViewControllers
- Passagem de objeto
- Ciclo de vida de ViewController
- Swift
- UIKit
- Auto Layout
- UIScrollView
- UITextField
- UIStackView

---

## 🔵 Tela 3 — Resultado da Simulação

Objetivo:  
Exibir os resultados do cálculo.

Elementos esperados:

- Valor final acumulado com destaque principal
- Total investido
- Lucro obtido
- Área de resumo com informações detalhadas

---

### 🧩 Componente — Resumo

Este componente deve:

- Receber os dados da simulação
- Exibir informações detalhadas
- Ser criado como uma `UIView` reutilizável ou como um método separado de configuração da interface
- Manter a tela de resultado mais organizada

Tecnologias aplicadas:

- Criação de componente com `UIView`
- Passagem de dados para componentes
- Organização modular da interface
- UIKit
- Auto Layout
- UIStackView

---

# 🧮 Regras de Cálculo

Utilize a fórmula de juros compostos:

```swift
M = P * pow(1 + i, t)
