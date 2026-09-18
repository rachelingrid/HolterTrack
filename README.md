# HolterTrack

**Diário digital de atividades para monitorização Holter**

O **HolterTrack** é um projeto de aplicativo voltado ao registro cronológico de atividades e eventos relevantes durante a monitorização por Holter.

A proposta inicial é substituir ou complementar o diário manual tradicional por um registro digital simples, padronizado e com marcação automática de data e hora.

> **Status do projeto:** protótipo em desenvolvimento — Versão 1 (V1)  
> **Repositório:** privado  
> **Licenciamento:** software proprietário — todos os direitos reservados

---

## Objetivo

Criar uma ferramenta simples que permita ao usuário registrar eventos cotidianos durante o período de monitorização Holter, gerando ao final uma linha do tempo organizada para auxiliar a correlação entre atividades relatadas e o registro eletrocardiográfico.

Nesta primeira versão, todos os eventos são registrados manualmente pelo usuário.

---

## Eventos da Versão 1

O HolterTrack V1 permite registrar:

- Refeição
- Caminhou
- Atividade física leve
- Atividade física moderada
- Atividade física de resistência
- Início do sono
- Despertar
- Medicação

Ao selecionar **Medicação**, o usuário deverá informar qual medicamento foi utilizado.

---

## Informações registradas

Cada evento contém:

- Data
- Hora
- Tipo de evento
- Detalhes adicionais, quando aplicável
- Timestamp completo para futura sincronização computacional

Exemplo:

```text
10/09/2026 | 08:02:41 | MEDICAÇÃO | Losartana 50 mg
10/09/2026 | 09:16:20 | CAMINHOU
10/09/2026 | 12:43:02 | REFEIÇÃO
```

---

## Funcionamento da V1

```text
Usuário realiza uma atividade
        ↓
Seleciona o evento no HolterTrack
        ↓
O aplicativo registra automaticamente
data + hora + tipo do evento
        ↓
Os dados são armazenados localmente
        ↓
Ao final do exame
        ↓
É gerado um relatório cronológico
```

---

## Saídas previstas

A Versão 1 deverá permitir:

- visualização da linha do tempo de eventos;
- armazenamento local dos registros;
- exportação dos dados em CSV;
- impressão ou salvamento do relatório em PDF.

---

## Tecnologias iniciais

O primeiro protótipo será desenvolvido com:

- HTML
- CSS
- JavaScript
- LocalStorage

A proposta é que a primeira versão possa funcionar diretamente no navegador e sem necessidade de servidor para o registro básico dos eventos.

---

## Estrutura inicial do projeto

```text
holter-track/
│
├── index.html
└── README.md
```

Com a evolução do projeto, a estrutura poderá ser separada em arquivos específicos:

```text
holter-track/
│
├── index.html
├── style.css
├── app.js
├── README.md
└── assets/
```

---

## Roadmap

### V1 — Diário manual

- Registro manual de atividades
- Data e hora automáticas
- Registro de medicação com descrição obrigatória
- Armazenamento local
- Relatório cronológico
- Exportação CSV
- Impressão/PDF

### V2 — Registro de duração

- Início e término de caminhada
- Início e término de atividade física
- Cálculo automático da duração dos eventos

### V3 — Recursos do smartphone

- Contagem de passos
- Acesso a sensores de movimento
- Identificação assistida de caminhada e corrida

### V4 — Automação

- Reconhecimento automático de atividades
- Estimativa de períodos de repouso
- Detecção assistida de sono e despertar
- Classificação de eventos por nível de confiança

### V5 — Integração temporal

- Exportação padronizada de eventos
- Sincronização da linha temporal com dados provenientes do Holter
- Ferramentas para correlação entre eventos e alterações eletrocardiográficas

---

## Princípio do projeto

O HolterTrack não pretende interpretar o eletrocardiograma na sua versão inicial.

Seu objetivo é produzir um **registro temporal estruturado dos eventos vivenciados pelo usuário durante a monitorização**, permitindo que essas informações sejam posteriormente comparadas com o traçado do Holter.

---

## Privacidade

Na versão inicial, os dados serão armazenados localmente no dispositivo do usuário.

O projeto deverá evoluir adotando princípios de minimização de dados, segurança da informação e proteção de dados pessoais.

---

## Aviso

O HolterTrack é atualmente um **projeto experimental em desenvolvimento**.

Não substitui avaliação médica, interpretação especializada do Holter ou sistemas médicos validados. Qualquer uso clínico futuro dependerá de desenvolvimento, testes, validação e adequação às exigências regulatórias aplicáveis.

---

## Licença e direitos autorais

**HolterTrack é um software proprietário em desenvolvimento.**

Copyright © 2026 Rachel Ingrid Pereira da Rocha Jannuzzi.  
**Todos os direitos reservados.**

Este repositório não é distribuído sob uma licença open source.

Nenhuma permissão é concedida, de forma expressa ou implícita, para copiar, reproduzir, modificar, redistribuir, sublicenciar, publicar, disponibilizar, comercializar ou criar trabalhos derivados do código-fonte, documentação, estrutura, interface ou demais materiais deste projeto sem autorização prévia e expressa da autora.

O acesso ao repositório privado não implica cessão ou concessão de quaisquer direitos de propriedade intelectual.

Qualquer futura alteração do regime de licenciamento deverá ser formalmente indicada neste repositório.

Copyright (c) 2026 Rachel Ingrid. All rights reserved.

This source code and related documentation are the confidential and proprietary information of the author. 
Unlicensed copying, distribution, modification, or public display via any medium is strictly prohibited.

---

## Autoria

Projeto **HolterTrack**

Desenvolvido como projeto experimental para estudo de tecnologias aplicadas à monitorização e ao registro de atividades durante exames de Holter.

---

## Versão

**HolterTrack V1 — protótipo inicial**
