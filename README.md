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

Estudante de **Ciência da Computação na PUC Minas** e desenvolvedor na
**[Tecwise Latam](https://br.linkedin.com/company/tecwiselatam)**, onde trabalho com
**IoT e monitoramento geotécnico** — piezômetros, células de carga e crackmeters
instalados em campo.

Atuo nas duas pontas da cadeia. Na entrada, o **TWBridge**: a ferramenta que lê o
arquivo bruto do sensor e o entrega ao broker sem perder medição. Na saída, o
**TWMonitor**, plataforma **white-label** da empresa construída sobre o motor do
**ThingsBoard PE** — onde eu construo as **rule chains** que processam e roteiam
a telemetria, os **alarmes** por limiar e os **dashboards** que o cliente usa.

É um domínio onde perder uma medição não é bug cosmético — é um dado de segurança
que deixou de existir. Essa restrição moldou como eu escrevo software.

<br/>

## Do sensor ao painel

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/pipeline-dark.svg">
  <img src="./assets/pipeline-light.svg" alt="Pipeline de telemetria: sensor em campo, ingestão pelo TWBridge, broker MQTT e a plataforma TWMonitor sobre ThingsBoard PE, com rule chains, alarmes e dashboards. Quando a rede cai, as medições vão para uma fila em disco e são reenviadas ao reconectar." width="100%">
</picture>

Duas coisas neste desenho são o meu trabalho.

A primeira é o **caminho tracejado**: quando a rede cai, as medições vão para uma
fila em disco e são reenviadas sozinhas ao reconectar. Sem ele, cada instabilidade
de conexão vira um buraco permanente na série temporal. Com ele, vira um atraso.

A segunda é o que está **dentro do TWMonitor**. O ThingsBoard entrega o motor;
a lógica que transforma leitura crua em informação útil — qual regra dispara qual
alarme, como a telemetria é roteada e enriquecida, o que o cliente enxerga no
painel — é construída por cima, e é aí que fica a maior parte do meu dia.

<br/>

## Stack

<div align="center">

**Linguagens**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)

**Frameworks**

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=threedotjs&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=for-the-badge&logo=nodedotjs&logoColor=white)

**IoT, nuvem & dados**

![MQTT](https://img.shields.io/badge/MQTT-660066?style=for-the-badge&logo=mqtt&logoColor=white)
![ThingsBoard](https://img.shields.io/badge/ThingsBoard-2F4F7F?style=for-the-badge&logo=thingsboard&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![Locust](https://img.shields.io/badge/Locust-0B6B8F?style=for-the-badge&logo=locust&logoColor=white)

**Ferramentas**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)

</div>

<br/>

## Projetos em destaque

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

### 📡 TWBridge + TWMonitor
**Python · MQTT · ThingsBoard PE** · 🔒 trabalho interno

O diagrama acima, em produção na Tecwise Latam.

**TWBridge** — lê o arquivo bruto do sensor, converte para JSON e publica via MQTT sobre TLS. Se a rede cai, **enfileira em disco e reenvia sozinho**. Empacotado como instalador Windows para equipe de campo.

**TWMonitor** — plataforma white-label sobre o motor do ThingsBoard PE, onde construo as **rule chains**, os **alarmes** por limiar e os **dashboards** entregues ao cliente.

`mqtt` · `iot` · `rule-chains` · `dashboards`

</td>
<td width="50%" valign="top">

### 💰 Análise Financeira Empresarial
**Python (stdlib pura) · SQLite** · 🔒 privado

Importa extrato OFX, classifica lançamentos por regras que o usuário ensina, e apura **DRE, fluxo de caixa, depreciação, ponto de equilíbrio e Simples Nacional**. Aritmética em **centavos inteiros** — rateio sem perder um centavo. Zero dependências externas.

`fintech` · `ofx` · `contabilidade` · `zero-deps`

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
<sub>Os projetos marcados com 🔒 envolvem dados de clientes, trabalho interno ou repositório fechado da universidade. Posso apresentá-los em conversa.</sub>
</div>

<br/>

## Contato

Aberto a oportunidades em **desenvolvimento de software, IoT e dados**. Se o problema envolve dado que não pode se perder, é o tipo de coisa que eu gosto.

<div align="center">

<a href="https://www.linkedin.com/in/samuelfalvesvieira">
  <img src="https://img.shields.io/badge/Chamar%20no%20LinkedIn-0B6B8F?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
</a>
<a href="mailto:samuelalvesvieira39@gmail.com">
  <img src="https://img.shields.io/badge/Mandar%20um%20email-12705A?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
</a>

</div>
