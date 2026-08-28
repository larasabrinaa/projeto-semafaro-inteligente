# 🚦 **Semáforo Inteligente com Arduino e Dashboard Web**

## 📌 Sobre o projeto

O **Semáforo Inteligente** é um projeto acadêmico desenvolvido com o objetivo de simular um sistema de controle de tráfego utilizando **Arduino, sensor e uma interface web (Dashboard)**.

O sistema permite visualizar o funcionamento do semáforo em tempo real, registrar eventos de detecção e simular situações de falha.

---

## 🎯 Objetivos

- Desenvolver um sistema de semáforo automatizado.
- Integrar o Arduino com uma interface web.
- Detectar a presença de objetos através de um sensor.
- Controlar a sequência das luzes do semáforo.
- Registrar os eventos de detecção.
- Simular uma situação de falha do sistema.
- Demonstrar o funcionamento do sistema através de um Dashboard Web.

---

## ⚙️ Funcionamento

O sistema possui três estados principais:

🟢 **Verde**  
Indica que o trânsito está liberado.

🟡 **Amarelo**  
Indica atenção e prepara o sistema para fechar o sinal.

🔴 **Vermelho**  
Indica que o trânsito deve parar.

Quando um objeto é detectado, o sistema realiza automaticamente a sequência:

**🟢 Verde → 🟡 Amarelo → 🔴 Vermelho → 🟢 Verde**

O sinal permanece no amarelo durante aproximadamente **7 segundos** e, em seguida, entra no vermelho durante **15 segundos**, realizando uma contagem regressiva no Dashboard.

Após o término da contagem, o sistema retorna ao sinal verde.

---

## 🤖 Integração com Arduino

O Dashboard Web possui comunicação com o Arduino através da **Web Serial API**.

Quando o Arduino envia a informação:

`DETECTADO`

o Dashboard interpreta o comando e inicia automaticamente a sequência do semáforo.

A comunicação serial é configurada com:

- **Baud rate:** 9600
- **Comunicação:** USB / Serial
- **Navegador recomendado:** Google Chrome ou Microsoft Edge

---

## ⚠️ Simulação de Falha

O projeto também possui uma função para simular uma falha no sistema.

Ao selecionar **"⚠️ Simular Falha"**:

- O funcionamento normal do semáforo é interrompido.
- O sinal amarelo passa a piscar.
- O sistema informa que está inoperante.
- O acionamento do sensor é bloqueado.
- A falha é registrada no histórico de eventos.

Após selecionar **"✅ Restaurar Semáforo"**, o sistema retorna ao funcionamento normal e o sinal verde é acionado.

---

## 📋 Registro de Eventos

O Dashboard possui um histórico que registra os principais eventos do sistema.

Entre os eventos registrados estão:

- 🚗 Detecção de objeto
- ⚠️ Falha no sistema
- ✅ Restauração do sistema

Cada evento recebe automaticamente o horário em que ocorreu.

---

## 💻 Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript
- Arduino
- Web Serial API
- Sensor de detecção
- GitHub

---

## 🖥️ Dashboard Web

A interface web apresenta:

- 🚦 Semáforo visual
- ⏱️ Contagem regressiva
- 🔌 Conexão com Arduino
- 🚗 Simulação de detecção
- ⚠️ Simulação de falha
- 📋 Registro de eventos

---

## 📷 Imagens do projeto

### Montagem e desenvolvimento

As imagens abaixo apresentam registros do desenvolvimento e funcionamento do projeto.

![Imagem do projeto](<Captura de tela 2026-08-28 155548.png>)

![Imagem do projeto](<Captura de tela 2026-08-28 155706.png>)

---

## 🎥 Demonstração

Foi realizada uma gravação da tela para demonstrar o funcionamento da simulação do semáforo através do Dashboard Web.

🎬 [Assistir à demonstração](<Gravação de Tela 2026-08-28 163242.mp4>)

---

## 📄 Documentação

Os documentos utilizados durante o desenvolvimento e apresentação do projeto estão disponíveis abaixo.

📑 [Apresentação do projeto](<SmartLight - Apresentação.pdf>)

📑 [Relatório de Execução Final](<Relatorio de Execução Final.pdf>)

---

## 🚀 Como executar

### 1. Baixe ou clone este repositório

### 2. Abra o arquivo:

`index.html`

### 3. Execute o arquivo em um navegador compatível

Recomenda-se utilizar:

- Google Chrome
- Microsoft Edge

### 4. Teste a simulação

Clique em:

**"Simular no Web"**

para iniciar o funcionamento do semáforo.

Também é possível utilizar:

**"⚠️ Simular Falha"**

para testar o comportamento do sistema em uma situação de falha.

---

## 🔌 Funcionamento com Arduino

Para utilizar a integração com o Arduino:

1. Conecte o Arduino ao computador através do USB.
2. Abra o `index.html` no navegador compatível.
3. Clique em **"🔌 Conectar ao Arduino"**.
4. Selecione a porta serial correspondente ao Arduino.
5. O sistema estará pronto para receber os dados do sensor.

Quando o Arduino enviar o comando `DETECTADO`, o Dashboard iniciará a sequência do semáforo.

---

## 👥 Equipe

**Projeto acadêmico desenvolvido para estudo e aplicação prática de conceitos de automação, programação e sistemas embarcados.**

---

## 📚 Documentação adicional

Este repositório contém:

- Código-fonte do Dashboard Web
- Imagens do projeto
- Apresentação em PDF
- Relatório de execução
- Vídeo demonstrativo

---

## 📜 Licença

Este projeto está disponível sob a licença **MIT**.
