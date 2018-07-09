---
layout: post
title: "Estudo da lista de utentes 2"
excerpt: "Criação das tabelas em excel"
categories: [PowerBi]
tags: [PowerBi, código]
comments: false
image:
  feature: header_powerbi.jpg
---

obter dados - excel - ligar
* seleccionar "problemas.xlsx"
- tabela 1
- editar
- abrir a janela do PowerQuery se esta ficar em segundo plano
- mudar o nome de tabela1 para Problemas
* nova origem - excel - abrir o ficheiro "utentes"
- seleccionar Tabela 1 -> ok
- mudar o nome de tabela1 para Utentes
- converter coluna utente para texto -> substituir a actual
* fechar e aplicar
Utentes - Idade
* criar grupos
  - tipo de grupo: discretizar com tamanho 5

* introduzir as measures/medidas (processo tedioso)

* distribuiçao por sexos
  - gráfico circular
  -- Detalhes: Sexo
  -- Valores: Sexo (Contagem de)
 - formatar cores de dados
-- Mulher FFC0CB
-- Homem 00BFFF

* Indices
- Matriz
--Valores: Burgdofer; Friz; Sauvy; Sundbarg
--Formatar -> Valores -> Mostrar nas linhas (activar)
-- redimensionar

* Repetir em nova matriz para os outros indices

* Piramide etária:
- importar visual personalizado (importar do marketplace)
- procurar -> tornado -> Tornado Chart -> adicionar

* tornado Chart
- grupo: idade (posições armazéns) - ou "bins"
- Legenda: Sexo
- valores: Utente (contagem de)
--formatar as cores

Nova Página
* Gráfico de colunas empilhadas
- eixo: capitulo
- Valor: quantidade de problemas
- formatar: etiquetas de dados: activo

* Gráfico de colunas empilhadas
- eixo: ICPC
- Valor: quantidade de problemas
- formatar: etiquetas de dados: activo
-- Filtros: ICPC: TOP N (15) pelo valor Qtd de problemas -> aplicar filtro
*Formato -> editar interacções
-seleccionar primeiro gráfico; clicar em filtrar no segundo
