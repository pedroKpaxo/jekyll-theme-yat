---
layout: post
title: Uma breve história da Perfilagem digital
subtitle: DOs irmãos Schlumberger aos arquivo .LAS
categories: markdown
tags: [Geologia design]
---

# Introdução

Um pequeno resumo dos avanços no campo da perfilagem digital.
Base para os próximos trabalhos.


# Perfis_Digitais

**Conrad e Marcel Schlumberger**, que fundaram a **Schlumberger Limited em 1926**, são considerados os inventores da perfilagem elétrica de poços.
Conrad desenvolveu a matriz Schlumberger, que era uma técnica de prospecção de depósitos de minério de metal, e os irmãos adaptaram essa técnica de superfície para aplicações subterrâneas.

Em 5 de setembro de 1927, uma equipe que trabalhava para a Schlumberger Limited baixou uma sonda elétrica acoplada a sua matriz em um poço localizado em **Pechelbronn**, Alsácia, França, criando o primeiro perfil de poço. Em termos modernos, o primeiro registro era um registro de resistividade que poderia ser descrito como registro lateral invertido de 3,5 metros. 

### A era digital

Uma operação típica de perfilagem cria múltiplas curvas de medição ao longo de extensos comprimentos de furo. Consequentemente, os dados de registro são numerosos e numéricos e são candidatos óbvios para armazenamento e processamento em  computadores.

A industria do óleo e gás acompanhou a evolução da computação, passando de um armazanemnto direto dos dados onde os perfis eram impressos e o gráfico representava seu produto final, para o armazenamento em fitas e depois do 


### Arquivos .Lis

**Log Interchange Standard (LIS)** é o predecessor do DLIS e foi desenvolvido pela Schlumberger no final dos anos 1970.
Como o DLIS, o LIS é um formato binário (big-endian). Ele é baseado no padrão de informações binárias VAX e tem uma sintaxe ainda mais estranha do que o DLIS.
Mesmo assim, os arquivos LIS ainda estão sendo produzidos e grandes volumes de informações de registro histórico existem neste formato. O Log I / O é uma plataforma conveniente para gerenciar e manter essas informações.
Um arquivo LIS físico consiste em um ou mais arquivos LIS lógicos, cada um contendo um conjunto de registros (metadados) de diferentes tipos, bem como uma curva de índice e um conjunto de curvas de medição. Cada curva pode ter uma ou várias amostras por medida de profundidade e, além disso, as curvas podem ser unidimensionais ou multidimensionais.

### Arquivos .Dlis

**Dlis** é um formato de arquivo binário para registros de poços, desenvolvido pela Schlumberger no final dos anos 80 e publicado pelo American Petroleum Institute (API) em 1991. Em 1998, a administração foi entregue à Petrotechnical Open Software Corporation (POSC), agora conhecida como energética 1

Ao desenvolver o padrão **dlis**, a ênfase principal foi colocada na escrita fácil. Os arquivos são estruturados de forma que os dados possam ser gravados diretamente durante a aquisição dos logs. Isso é muito útil para os produtores dos arquivos e igualmente tedioso para o consumidor que deseja lê-los mais tarde. Além disso, é um padrão muito tolerante. Ele especifica estruturas de dados gerais dentro do arquivo, como canais e quadros, mas permite que os produtores os modifiquem para atender às suas necessidades. Também permite estruturas completamente novas, não definidas pelo próprio padrão, como tipos de objeto específicos do fornecedor. Isso tudo se resume a um padrão bastante complexo, com muitas peculiaridades e estranhezas. É seguro dizer que dl é um formato particularmente difícil de trabalhar

### Arquivos .LAS

Quando os computadores pessoais tomaram o lugar dos mainframes na década de 1980, o meio de armazenamento de log digital mudou das fitas para os disquetes. As limitações de espaço dos primeiros PCs levaram ao desenvolvimento do formato **LAS (Log Ascii Standard)** pela Canadian Well Logging Society como uma maneira simples de codificar os logs que ocorrem com mais frequência e agora é um padrão usado em todo o mundo.