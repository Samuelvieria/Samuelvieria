<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/banner-dark.svg">
  <img src="./assets/banner-light.svg" alt="Samuel Alves Vieira — Desenvolvedor de Software · IoT e Telemetria" width="100%">
</picture>

<br/>

<a href="https://www.linkedin.com/in/samuelfalvesvieira">
  <img src="https://img.shields.io/badge/LinkedIn-Conectar-0B6B8F?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
</a>
<a href="mailto:samuelalvesvieira39@gmail.com">
  <img src="https://img.shields.io/badge/Email-Falar%20comigo-12705A?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
</a>
<a href="https://github.com/Samuelvieria?tab=repositories">
  <img src="https://img.shields.io/badge/Projetos-Ver%20todos-0B1219?style=for-the-badge&logo=github&logoColor=white" alt="Repositórios">
</a>

</div>

<br/>

## Sobre

Estudante de **Ciência da Computação na PUC Minas**. Na
**[Tecwise Latam](https://br.linkedin.com/company/tecwiselatam)** trabalho com IoT e
monitoramento geotécnico: desenvolvo a ingestão de telemetria dos sensores em campo e
atuo no desenvolvimento do **TWMonitor**, a plataforma de monitoramento construída
sobre ThingsBoard, onde implemento rule chains, alarmes e dashboards.

Fora disso, construo o que me interessa — e é onde passo o tempo que sobra: um globo 3D
que digere livros de história, um app offline-first para oficina mecânica, um sistema de
análise financeira sem uma única dependência externa.

O que atravessa tudo é um gosto por software que continua correto quando as condições
não são ideais.

<br/>

## Projetos

<table>
<tr>
<td width="50%" valign="top">

### [🌍 Globo Histórico Interativo](https://github.com/Samuelvieria/world-history-map)
**React 19 · TypeScript · Three.js · Python**

Globo 3D navegável onde eventos históricos viram pontos clicáveis, com navegação **mundo → continente → país → estado** e nível de detalhe progressivo.

Alimentado por um pipeline próprio que lê livros de história em PDF **sem usar LLM generativo** — modelos encoder que só apontam trechos existentes não conseguem fabricar um fato. Medido contra dois livros inteiros: **100% de proveniência íntegra em 2053 candidatos**.

[![Repo](https://img.shields.io/badge/Ver_o_código-0B6B8F?style=flat-square&logo=github&logoColor=white)](https://github.com/Samuelvieria/world-history-map)
[![MIT](https://img.shields.io/badge/MIT-16715A?style=flat-square)](https://github.com/Samuelvieria/world-history-map/blob/master/LICENSE)

</td>
<td width="50%" valign="top">

### 🔧 Screw — gestão para oficinas
**Flutter · Firebase · SQLite · Azure Vision** · 🔒 privado

App mobile **offline-first** para oficinas mecânicas: clientes, veículos, ordens de serviço e orçamentos em PDF. Grava local no SQLite e sincroniza sozinho com o Firestore quando a conexão volta. Inclui **leitura de placa por câmera (OCR)**.

Trabalho interdisciplinar em equipe de 6, em repositório fechado da PUC Minas.

`offline-first` · `sync` · `ocr` · `pdf`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 💰 Análise Financeira Empresarial
**Python (stdlib pura) · SQLite** · 🔒 privado

Importa extrato OFX, classifica lançamentos por regras que o usuário ensina, e apura **DRE, fluxo de caixa, depreciação, ponto de equilíbrio e Simples Nacional**. Aritmética em **centavos inteiros** — rateio sem perder um centavo. Zero dependências externas.

`fintech` · `ofx` · `contabilidade` · `zero-deps`

</td>
<td width="50%" valign="top">

### 🎬 VideosAut — pipeline de conteúdo
**Python · TTS · automação**

Pipeline por fases para produção de vídeo: roteiro, síntese de voz e render. Construído deliberadamente de trás pra frente — os primeiros vídeos são feitos à mão para descobrir o que funciona **antes** de automatizar qualquer etapa.

[![Repo](https://img.shields.io/badge/Ver_o_código-0B6B8F?style=flat-square&logo=github&logoColor=white)](https://github.com/Samuelvieria/VideosAut)

</td>
</tr>
</table>

### Também no ar

| Repositório | O que é |
|---|---|
| [**Engenharia de Software II**](https://github.com/Samuelvieria/Engenharia-De-software-II) | Sistema de biblioteca em Java — empréstimos, reservas e testes unitários com JUnit |
| [**TP AEDS III**](https://github.com/Samuelvieria/TP_AEDSIII) | Indexação e estruturas de dados em Java |
| [**DIW**](https://github.com/Samuelvieria/DIW) | Front-end de e-commerce em JS puro consumindo API REST |
| [**ACI**](https://github.com/Samuelvieria/ACI) | Circuitos digitais em Verilog |
| [**BD**](https://github.com/Samuelvieria/BD) | Modelagem relacional em MySQL e interface de acervo |

<div align="center">
<sub>Os projetos marcados com 🔒 envolvem dados de clientes ou repositório fechado da universidade. Posso apresentá-los em conversa.</sub>
</div>

<br/>

## Stack

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/stack-dark.svg">
  <img src="./assets/stack-light.svg" alt="Stack: Python, TypeScript, Java, JavaScript, Dart, C++, SQL · React, Three.js, Vite, Flutter, HTML/CSS · MQTT, ThingsBoard, SQLite, Firebase, Azure, Locust · Git, Linux, Docker, PyInstaller, Figma" width="100%">
</picture>

<br/>

## Um problema que eu gosto

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/pipeline-dark.svg">
  <img src="./assets/pipeline-light.svg" alt="Pipeline de telemetria: sensor, ingestão, broker MQTT e ThingsBoard com rule chains, alarmes e dashboards. Quando a rede cai, as medições vão para uma fila em disco e são reenviadas ao reconectar." width="100%">
</picture>

Sensor em campo, rede instável. O caminho sólido é o dia bom; o tracejado é o que
importa: **quando a conexão cai, a medição vai para uma fila em disco e é reenviada
sozinha ao reconectar.**

Sem isso, cada instabilidade vira um buraco permanente na série temporal. Com isso,
vira um atraso. A diferença entre as duas parece pequena no código e é enorme para
quem depende do dado.

<br/>

## Contato

<div align="center">

<a href="https://www.linkedin.com/in/samuelfalvesvieira">
  <img src="https://img.shields.io/badge/Chamar%20no%20LinkedIn-0B6B8F?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
</a>
<a href="mailto:samuelalvesvieira39@gmail.com">
  <img src="https://img.shields.io/badge/Mandar%20um%20email-12705A?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
</a>

</div>
