# GS-Edge-Computing

Repositório Global Solution - Edge Computing &amp; Computer Systems

---

### Link Simulação Wokwi

* https://wokwi.com/projects/465295052268670977

---

## Integrantes

* Alessandro Malarenko Scarcella - RM:567769
* Caio Issao Yokohama - RM:569606
* Daniel Taniwaki Pereira - RM:569424
* Lucas Narimatsu Namba - RM:569274
* Pedro Kazumy Lima Watanabe - RM:569165

---

## Descrição do Projeto

Este projeto é sobre um sistema inteligente de monitoramento climático para a agricultura, feito
com Arduino. Ele usa um sensor DHT22 para medir a temperatura e a umidade do ar em tempo
real. Os dados coletados são exibidos em um display LCD, permitindo que o usuário veja
facilmente as condições ambientais.
Quando os valores de temperatura ou umidade mostram que as condições não são ideais para o
cultivo, o sistema liga automaticamente uma irrigação simulada por meio de um servo motor.
Além disso, um LED vermelho se acende e uma mensagem de alerta aparece no display.
Quando as condições estão boas, o sistema mantém a irrigação desligada e sinaliza isso com um
LED verde.

---

## Objetivo da Solução

O objetivo deste projeto é ajudar agricultores a monitorar as condições climáticas e tomar
decisões sobre a irrigação.
A solução visa:
* Monitorar temperatura e umidade em tempo real;
* Automatizar a irrigação;
* Reduzir o desperdício de água;
* Facilitar o acompanhamento das condições ambientais;
* Mostrar como tecnologias inteligentes podem ser usadas na agricultura.

---

## Componentes Utilizados
Para fazer o projeto, foram usados os seguintes componentes:
* 1 Arduino Uno;
* 1 Sensor DHT22;
* 1 Display LCD 16x2 com módulo I2C;
* 1 Servo Motor SG90;
* 1 LED Verde;
* 1 LED Vermelho;
* 2 Resistores;
* 1 Half Breadboard;
* Cabos Jumpers para conexão.

---

## Funcionamento do Sistema

O sensor DHT22 lê continuamente a temperatura e a umidade do ar.
Quando a temperatura é menor ou igual a 30°C e a umidade é maior ou igual a 40%, o sistema
considera que as condições estão boas para o cultivo. Nesse caso, o LED verde fica aceso, o
servo motor fica parado e o display mostra a mensagem “Condições ideais".
Quando a temperatura passa de 30°C ou a umidade fica abaixo de 40%, o sistema identifica uma
situação de risco para a plantação. O LED vermelho se acende, o display informa que as
condições estão ruins e, após alguns segundos, mostra a mensagem “Ativando irrigação". Em
seguida, o servo motor gira, simulando a abertura de um sistema de irrigação.

---

## Estrutura do Circuito

As conexões do circuito foram feitas da seguinte forma:

### Sensor DHT22

* VCC conectado ao 5V do Arduino;
* DATA conectado ao pino digital 13;
* GND conectado ao GND.

### Servo Motor

* Pino de sinal conectado ao pino digital 3;
* Alimentação conectada ao 5V;
* GND conectado ao GND.

### LED Verde

* Terminal positivo conectado ao pino digital 10;
* Terminal negativo conectado ao GND através de um resistor.

### LED Vermelho

* Terminal positivo conectado ao pino digital 5;
* Terminal negativo conectado ao GND através de um resistor.

### Display LCD I2C

* VCC conectado ao 5V;
* GND conectado ao GND;
* SDA conectado ao pino A4;
* SCL conectado ao pino A5.

---

## Aplicação na Agricultura

Este sistema pode ser usado como uma solução de apoio ao agricultor, permitindo o
monitoramento constante das condições climáticas e ajudando no controle da irrigação. Dessa
forma, é possível reduzir desperdícios de água, melhorar a eficiência do cultivo e aumentar a
produtividade agrícola.

---
