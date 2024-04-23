# Projeto de IoT com Node-RED e Arduino

## Descrição

Este projeto consiste em um sistema de monitoramento utilizando os sensores DHT11 (para medição de temperatura e umidade) e 10I9 (sensor específico do projeto, ajuste conforme a aplicação real), integrados através de um Arduino e gerenciados pelo Node-RED. Os dados dos sensores são lidos a cada 3000ms e enviados para um broker MQTT, onde podem ser visualizados e monitorados através de um dashboard na plataforma TAGO.IO.

## Componentes

- Arduino UNO
- Sensor DHT11
- Sensor 10I9
- Computador com Node-RED instalado
- Acesso à Internet para conexão com MQTT broker e TAGO.IO

## Configuração

### Hardware

1. Conecte o sensor DHT11 à porta digital do Arduino.
2. Conecte o sensor 10I9 à outra porta digital do Arduino.
3. Certifique-se de que o Arduino está conectado ao computador via USB.

### Software

#### Configuração do Arduino

1. Carregue o código padrão para leitura dos sensores DHT11 e 10I9 no Arduino.
2. Certifique-se de que o Arduino esteja configurado para enviar os dados pela porta serial em formato JSON.

#### Configuração do Node-RED

1. Instale o Node-RED no seu computador.
2. Use os nós de entrada serial para ler os dados do Arduino.
3. Adicione nós para formatação dos dados em JSON conforme os requerimentos.
4. Configure os nós MQTT para conectar-se ao seu broker MQTT escolhido.
5. Defina os tópicos MQTT conforme a estrutura `fiap/iot/Turma/Grupo/Sensor`.

#### Configuração do Dashboard

1. Crie uma conta na plataforma TAGO.IO.
2. Configure um dashboard para visualizar os dados recebidos dos sensores.
3. Adicione widgets correspondentes a cada tipo de dado recebido (temperatura, umidade, e outros dados do sensor 10I9).

## Uso

Para visualizar os dados, abra o dashboard no TAGO.IO. Os dados dos sensores serão atualizados automaticamente a cada 3000ms conforme enviados pelo Node-RED ao broker MQTT e, posteriormente, captados pela plataforma.

## Contribuição

Para contribuir com o projeto, por favor envie suas sugestões e modificações via pull requests no repositório do GitHub associado ao projeto.


## Membros

Diana Letícia de Souza Inocencio 

Erick Molina Barreiros

Caio Hideki 

João Viktor Carvalho de Souza

Jorge Henrique Booz
