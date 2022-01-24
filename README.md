# Biblioteca Serial Debug para Arduino Due
[![platform badge](https://img.shields.io/badge/platform-Arduino-orange.svg)](https://github.com/arduino)
[![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/JoaoLopesF/SerialDebug/blob/master/LICENSE.txt)

## Contents

- [Sobre](#sobre)
- [Comandos Básicos](#comandos)
- [Como Utilizar](#como-utilizar)
- [Possíveis Atualizações](#implementações-futuras)

## Sobre

A IDE oficial do Arduino não possui depurador. Por isso, geralmente usa-se mensagens Serial como forma de depuração no Arduino, como *Serial.print(...)*.

Neste aspecto, serial_debug é uma biblioteca que fornece macros e funções para auxiliar na depuração serial para Arduino, sem a necessidade de hardware extra para isso.

## Comandos
### Macros:
- **DEBUG():** funciona como *Serial.print()*. Envia uma mensagem serial que pode ser visualizada em serial monitor.
- **DEBUGLN():** funciona como *Serial.println()*. Envia uma mensagem serial seguida de uma linha em branco, que pode ser visualizada em serial monitor. 
- **SEPARATOR():** Usado para imprimir na tela vários "-", a fim de separar visualmente conteúdos de mensagens.
- **DEBUG_- PRINT_FILE():** mostra o nome do arquivo referente ao código que está sendo executado no momento.
- **DEBUG_PRINT_LINE():** mostra a linha do arquivo referente ao código que está sendo executado no momento.
- **DEBUG_PRINT_PRETTY_FUNCTION():** mostra o nome da função no qual o código que está sendo executado no momento pertence.
- **PRINTVARIABLE(variableName, variable):** mostra o nome e o valor de uma variável.

### Funções:
- **debugTime:** mostra o tempo de execução até o momento, no formato: horas:minutos:segundos:milissegundo  
- **debugTimeBreak:** espera receber uma mensagem, por default 5 segundos. Após esse tempo a mensagem recebida é, então, enviada via serial para ser visualizada no serial monitor.

## Como utilizar

- Baixe.

<p align="center"> 
<img src="https://github.com/SciCoBot/serial_debug/blob/main/images/telaRespositorioBaixar.png" alt="Repositório Baixar" width="600"/>
</p>

- Adicione a partir da IDE arduino.

<p align="center"> 
<img src="https://github.com/SciCoBot/serial_debug/blob/main/images/telaArduino.png" alt="Tela Aruino" width="600"/>
</p>

- Teste o exemplo.

## Implementações futuras
- Testes automáticos.

