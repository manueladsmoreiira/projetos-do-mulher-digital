# Laboratório 3 — Rede SOHO

## Objetivo

O laboratório tem como objetivo construir e configurar uma rede SOHO aplicando conceitos básicos de redes de computadores, incluindo conexões cabeadas e sem fio, configuração de rede Wi-Fi, distribuição automática de endereços IP por DHCP e testes de conectividade.

## O que é uma rede SOHO?

A rede SOHO (Small Office/Home Office) é uma rede projetada para pequenos escritórios ou ambientes residenciais. 

## Topologia

- 1 nuvem (Cloud-PT), simulando a infraestrutura do provedor de Internet;
- 1 modem a cabo (Cable Modem);
- 1 roteador wireless WRT300N;
- 2 computadores (PCs) conectados via cabo Copper Straight-Through;
- 1 impressora de rede conectada via cabo Copper Straight-Through;
- 1 notebook conectado via Wi-Fi;
- 1 smartphone conectado via Wi-Fi.

A nuvem e o modem foram conectados usando cabo coaxial

## Etapas de Configuração

### 1. Montagem da Topologia

Os dispositivos foram adicionados à área de trabalho do Cisco Packet Tracer e organizados de acordo com o cenário proposto.

O modem foi conectado à nuvem, enquanto o roteador WRT300N foi conectado ao modem. Os computadores e a impressora foram ligados às portas Ethernet do roteador utilizando cabos Copper Straight-Through.

### 2. Configuração da Rede Wi-Fi

O roteador WRT300N foi configurado com os seguintes parâmetros:

| Parâmetro | Configuração |
|---|---|
| SSID | `Escritorio_Firma` |
| Segurança | WPA2-Personal |
| Senha de laboratório | `senha12345` |

### 3. Conexão dos Dispositivos Sem Fio

O smartphone foi configurado para acessar a rede `Escritorio_Firma` utilizando WPA2-PSK.

No notebook, foi realizada a substituição do módulo de rede cabeada por uma placa wireless WPC300N. Em seguida, o equipamento foi conectado à rede Wi-Fi por meio do aplicativo PC Wireless.

### 4. Configuração do DHCP

O servidor DHCP do roteador WRT300N foi utilizado para distribuir automaticamente endereços IP aos dispositivos da rede local.

Os computadores e a impressora foram configurados para obter seus endereços IP automaticamente. O notebook e o smartphone também foram configurados para utilizar DHCP, quando necessário.

O roteador utiliza, por padrão, a faixa de endereços `192.168.0.x`, podendo atribuir endereços diferentes a cada dispositivo.

### 5. Teste de Conectividade

Para verificar a comunicação entre os dispositivos, foi realizado um teste de conectividade utilizando o comando `ping`.

O teste foi executado no PC0, por meio do Command Prompt, utilizando o endereço IP atribuído à impressora.

```bash
ipconfig
ping <192.168.0.103>
```

O teste indicou conectividade entre os dispositivos na rede local.

## Resultados

*Adicione aqui uma captura de tela da topologia completa no Cisco Packet Tracer.*

![Topologia da rede SOHO](t.png)

### Configuração da Rede Wi-Fi

*Adicione aqui uma captura de tela das configurações de SSID e segurança do roteador WRT300N.*

<!-- Substitua pelo caminho da imagem no repositório -->
![Configuração da rede Wi-Fi](imagens/configuracao-wifi.png)

### Teste de Conectividade

*Adicione aqui uma captura de tela do Command Prompt mostrando o comando ping e as respostas recebidas.*

<!-- Substitua pelo caminho da imagem no repositório -->
![Teste de conectividade entre PC0 e a impressora](imagens/teste-ping.png)



## 🎯 Conclusão

Este laboratório permitiu praticar conceitos fundamentais de redes de computadores por meio da construção e configuração de uma rede SOHO no Cisco Packet Tracer. A atividade reuniu conhecimentos sobre topologia, conectividade, segurança Wi-Fi, endereçamento IP e testes de comunicação, simulando situações comuns na infraestrutura de um pequeno escritório.

