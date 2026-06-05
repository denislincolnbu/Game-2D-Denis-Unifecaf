
# Projeto Plataforma 2D - UNIFECAF

Este é um jogo de plataforma bidimensional desenvolvido como projeto final para a disciplina de Game Development do curso de Análise e Desenvolvimento de Sistemas do Centro Universitário UniFECAF.

O projeto foi construído utilizando a engine Unity (versão Unity 6) e programado inteiramente na linguagem C#, aplicando conceitos fundamentais de física 2D, gerenciamento de estados de animação, ciclo de vida de scripts (Game Loop) e interface de usuário.

---

## 📹 Demonstração em Vídeo

Assista ao vídeo pitch de apresentação do projeto, contendo a explicação técnica das mecânicas implementadas e a demonstração completa da gameplay:

👉 **[Clique aqui para assistir ao vídeo do projeto](https://youtu.be/ofk9RFDi8vk)**

---

## 🎮 Mecânicas e Funcionalidades

O jogo implementa os principais fundamentos exigidos para uma experiência completa de plataforma 2D:

* **Movimentação Física Responsiva:** Controle de deslocamento lateral baseado no componente `Rigidbody2D` com a propriedade `linearVelocity`, garantindo movimentos mais naturais e fluidos.
* **Sistema de Pulo Inteligente:** Impulso vertical com checagem de colisão no chão para evitar saltos infinitos no ar.
* **Coleta de Itens e Pontuação:** Moedas e estrelas espalhadas pelo cenário utilizam colisores em modo gatilho (*Triggers*) para registrar a coleta e atualizar o contador de pontos em tempo real.
* **Sistema de Dano e Limites de Mapa:** Caso o jogador caia em zonas de perigo ou fora dos limites inferiores do cenário, a fase é reiniciada automaticamente, e a pontuação é redefinida.
* **Progressão de Fases:** Estrutura dividida em 3 fases com curva de dificuldade crescente, desafiando a precisão dos saltos e a coordenação motora do jogador através do layout do cenário.
* **Feedback Visual e Sonoro:** Máquina de estados configurada no *Animator Controller* para transições entre *Idle*, *Walk* e *Jump*. Efeitos sonoros acionados via código para dar resposta imediata às ações de pulo e coleta.

---

## ⌨️ Controles do Jogo

As ações do personagem são controladas diretamente pelo teclado através dos seguintes comandos básicos:

| Ação | Teclas |
| :--- | :--- |
| **Mover para a Esquerda** | Seta Esquerda ou Tecla `A` |
| **Mover para a Direita** | Seta Direita ou Tecla `D` |
| **Pular** | Barra de Espaço (`Space`) |

---

## 📁 Estrutura do Repositório

O repositório está organizado para conter apenas os arquivos de desenvolvimento e o código-fonte essenciais da Unity:

* **`Assets/Scripts/`**: Contém todos os scripts desenvolvidos em C# (`Player`, `Coin`, `GameManager`, etc.) estruturados de forma limpa.
* **`Assets/Sprites/`**: Pacotes de imagens em duas dimensões organizados para o mapeamento de tiles e cenários.
* **`Assets/Animations/`**: Controladores e clipes de animação do personagem principal e elementos interativos.
* **`ProjectSettings/`**: Configurações internas do projeto Unity, como física de colisões e mapeamento de inputs.

---

## 🚀 Como Executar o Projeto

Para abrir e testar o projeto no seu ambiente de desenvolvimento, siga os passos abaixo:

1. Certifique-se de ter o **Unity Hub** e a versão **Unity 6 (6000.4.9f1)** ou superior instalada no computador.
2. Faça o clone deste repositório ou baixe a pasta do projeto.
3. No Unity Hub, clique em **Add** > **Add project from disk** e selecione a pasta raiz `Projeto Plataforma UNIFECAF Denis`.
4. Abra o projeto e, na aba *Project*, navegue até `Assets/Scenes/` e abra a cena inicial (`SampleScene`).
5. Clique no botão **Play** no topo da engine para testar o jogo diretamente pelo editor.
