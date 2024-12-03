### README

# 🏎️ Simulador de Corrida

Um jogo simples de simulação de corrida, desenvolvido em **JavaScript** e **Node.js**, onde dois personagens, **Mario** e **Luigi**, competem em cinco rodadas com diferentes desafios: **velocidade**, **manobrabilidade** e **poder**. 

## 🎮 Como funciona

1. O jogo é dividido em 5 rodadas.
2. Cada rodada sorteia um tipo de bloco: **reta**, **curva** ou **confronto**.
3. Os jogadores lançam um dado virtual para determinar seus resultados, que são somados ao atributo correspondente:
   - **Reta**: soma-se a **velocidade**.
   - **Curva**: soma-se a **manobrabilidade**.
   - **Confronto**: soma-se o **poder**.
4. No caso de "confronto", o jogador vencedor faz o adversário perder 1 ponto (se este tiver mais de 0 pontos).
5. Após todas as rodadas, o vencedor é o jogador com mais pontos acumulados.

## 🚀 Como executar

1. Certifique-se de ter o **Node.js** instalado no seu computador.
2. Clone este repositório ou copie o código do projeto.
3. Navegue até o diretório do projeto e execute o comando:
   ```bash
   node index.js
   ```
4. Observe a simulação da corrida diretamente no terminal.

## 📜 Regras do Jogo

- Cada jogador começa com 0 pontos.
- A cada rodada:
  - O bloco determina qual atributo será testado.
  - O vencedor da rodada ganha 1 ponto (exceto no confronto, onde o perdedor pode perder um ponto).
  - Empates não concedem nem retiram pontos.
- Ao final das 5 rodadas, o jogador com mais pontos vence.

## 🛠️ Estrutura do Código

- **Objetos de Jogadores**: Contêm atributos como nome, velocidade, manobrabilidade, poder e pontuação.
- **Funções Principais**:
  - `rollDice`: Simula o lançamento de um dado.
  - `getRandomBlock`: Sorteia o tipo de bloco da rodada.
  - `logRollResult`: Exibe os resultados do dado e o atributo utilizado.
  - `playRaceEngine`: Executa a lógica da corrida rodada por rodada.
  - `declareWinner`: Declara o vencedor após o término das rodadas.

## 🏆 Resultado

- O terminal exibirá o resumo das rodadas, os pontos de cada jogador e o vencedor final.

Divirta-se com este simulador de corrida virtual! 🚗💨

--- 

Se precisar de mais explicações ou melhorias, é só pedir! 😊
