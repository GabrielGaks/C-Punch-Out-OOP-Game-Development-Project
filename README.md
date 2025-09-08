# **C# Punch-Out Game | OOP + Windows Forms**

Um projeto de **desenvolvimento de jogos em C#**, inspirado no clássico *Punch-Out*, reformulado com **Programação Orientada a Objetos (POO)**, **Windows Forms** e **design moderno**.

Neste projeto, criei uma versão onde **grandes personalidades da computação** batalham entre si em combates 1x1. O objetivo foi **evoluir a arquitetura do código**, adicionar **novas funcionalidades** e melhorar a **experiência visual**, simulando um ciclo real de evolução de software.

---

## 🎮 Sobre o Projeto

A base do jogo era extremamente simples e limitada:
- Início direto do jogo (sem menus).
- Sprites de baixa qualidade.
- Sem seleção de personagens.
- Mecânica muito fácil.

### **Principais melhorias implementadas**
- **Interface (Windows Forms):**
  - Menu inicial com *Iniciar* / *Sair*.
  - Seleção de personagem com atributos e imagem.
  - Tela de combate com HUD (vida, força, velocidade).
  - Tela de resultado (vencedor, reiniciar, voltar ao menu).
- **Sistema de personagens:**
  - 4 personagens jogáveis.
  - **32 sprites originais** criados com IA (8 por personagem).
  - Atributos exclusivos: **Vida**, **Força**, **Velocidade** e **Defesa**.
- **Mecânica de bloqueio:**
  - Se **Defesa > Força do ataque inimigo**, o personagem **recupera vida**.
- **Código estruturado (POO):**
  - Classes para personagens, combate e fluxo de jogo.
  - Uso de **List** e **Dictionary** para gerenciamento dinâmico.
  - Código modular, preparado para expansão.

---

## 🗂 Estrutura do Projeto

```
Simple-Punch-Out-Game/
│
├── Properties/                 # Configurações do projeto
├── Resources/                  # Sprites e imagens
├── bin/                        # Artefatos compilados
├── obj/                        # Temporários de build
├── .gitignore                  # Arquivos ignorados
├── Simple Punch Out Game.sln   # Solução do Visual Studio
└── README.md                   # Este documento
```

---

## 💻 Tecnologias Utilizadas

- **Linguagem:** C#
- **Framework:** .NET (Windows Forms)
- **Paradigma:** Programação Orientada a Objetos (POO)
- **IDE:** Visual Studio
- **Outros:** Git/GitHub, IA para geração de sprites

---

## ⚙️ Como Executar

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/GabrielGaks/C-Punch-Out-OOP-Game-Development-Project.git
   ```
2. **Abra no Visual Studio:**
   - `Arquivo` → `Abrir` → `Projeto/Solução`
   - Selecione `Simple Punch Out Game.sln`
3. **Compile e execute:**
   - `Build > Build Solution` (`Ctrl + Shift + B`)
   - `Start` (`F5`)

---

## 🧠 Lógica de Jogo (Resumo Técnico)

- **Seleção de personagens:** carregada via `Dictionary<int, Personagem>` e navegação por índice com `List`.
- **Atributos por personagem:** `vida`, `forca`, `velocidade`, `defesa`.
- **Combate:** cálculo de dano considera força do atacante e defesa do defensor.
- **Bloqueio com recuperação:** se `defesa >= forcaInimigo`, aplica-se **cura** em vez de dano.
- **Fluxo de telas:** `Menu → Seleção → Combate → Resultado → (Menu/Replay)`.

---

## 📌 Backlog (Futuras Melhorias)

- **Ringue:** melhorar o design/estética da tela de luta.
- **Dificuldade/IA:** tornar a experiência mais desafiadora.
- **Mecânicas novas:** golpes especiais e movimentação livre pelo ringue.
- **Pausa:** implementar sistema de *pause/resume*.

---

## 🖼 Capturas de Tela

 # Menu Inicial
> <img width="1150" height="677" alt="image" src="https://github.com/user-attachments/assets/b0866d66-2bb8-49c7-b63f-8372c417436e" />

 # Seleção de Personagem
> <img width="1149" height="680" alt="image" src="https://github.com/user-attachments/assets/d84dd046-a754-4606-85a7-b47f2e3b370b" />
 # Combate
> <img width="834" height="592" alt="image" src="https://github.com/user-attachments/assets/56a5bc4d-1a75-4e8b-a63e-7a5adca712a9" />
 # Resultado
> <img width="802" height="479" alt="image" src="https://github.com/user-attachments/assets/b219246c-f9e5-4170-ba54-05fdbe7ce810" />

---

## 🌟 Objetivo do Projeto

Demonstrar:
- **Domínio de POO em C#** (classes, encapsulamento, listas/dicionários).
- **Organização e modularidade** do código.
- **UI/UX com Windows Forms**.
- Evolução de um projeto real com **mecânicas personalizadas**.

---

## 📄 Licença

Este projeto está sob a licença **MIT**.  
Sinta-se à vontade para usar, estudar e contribuir.

---

## 🤝 Contribuição

Contribuições são bem-vindas!  
Abra uma *issue* para sugestões, *bugs* ou novas ideias.

