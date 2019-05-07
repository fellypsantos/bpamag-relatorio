# bpamag-relatorio

Emissão de relatórios mais organizados do BPA Magnético
Esse script desenvolvido em python3 usa o Relatório de Produção Consolidada exportado pelo BPA Magnético nomeado "BPAC_REL.txt" para somar o total de cada procedimento realizado em um determinado estabelecimento de saúde.

### Relatório Consolidado

Por padrão do SUS, alguns procedimentos são consolidados por idade, esse script consolida de forma rápida e simples o Relatório Consolidado do BPA em um único total de vezes que cada procedimento foi realizado em um estabelecimento, independente da idade.

> **Arquivo BPA Magnético: BPAC_REL.txt**

Procedimento | CBO | Idade | Quantidade

:------------: | :----: | :-----: | :---------:

02.04.04.009-4 | 225142 | 028 | 7

02.04.04.009-4 | 225142 | 029 | 15

02.04.04.009-4 | 225142 | 030 | 6

> **Consolidado pelo: BPAC-PP**

Procedimento | Quantidade | Descrição

:------------: | :----: |:---------:

02.04.04.009-4 | 28 | RADIOGRAFIA DE MAO

---

### Requisitos de sistema

- Python3
