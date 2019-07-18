# bpamag-relatorio

Emissão de relatórios mais organizados do BPA Magnético

Esse script desenvolvido em python3 usa o Relatório de Produção Consolidada exportado pelo BPA Magnético nomeado "BPAC_REL.txt" para somar o total de cada procedimento realizado em um determinado estabelecimento de saúde.

### Modo de uso

```
python bpamag.py --arquivo nome_arquivo.txt
```

### Relatório Consolidado

Por padrão do SUS, alguns procedimentos são consolidados por idade, esse script consolida de forma rápida e simples o Relatório Consolidado do BPA em um único total de vezes que cada procedimento foi realizado em um estabelecimento, independente da idade.

> **Arquivo BPA Magnético: BPAC_REL.txt**

|  Procedimento  |  CBO   | Idade | Quantidade |
| :------------: | :----: | :---: | :--------: |
| 02.04.04.009-4 | 225142 |  028  |     7      |
| 02.04.04.009-4 | 225142 |  029  |     15     |
| 02.04.04.009-4 | 225142 |  030  |     6      |

> **Consolidado pelo bpamag.py**

|  Procedimento  | Quantidade | Val Unit | Val Total  |     Descrição      |
| :------------: | :--------: | :------: | :--------: | :----------------: |
| 02.04.04.009-4 |     28     | R\$ 6,30 | R\$ 176,40 | RADIOGRAFIA DE MAO |

---

### Rodando o script

1 - Gere um relatório consolidado dentro do BPA Magnético
![Exportando relatório no BPA-Magnético](https://i.imgur.com/bJQOkg6.gif)

2 - Copie o arquivo BPAC_REL.TXT pra dentro da pasta do bpamag.py e rode o comando.
![Executando script bpamag.py](https://i.imgur.com/7qZ7kDe.gif)

3 - Um relatório com descrição dos procedimentos será gerado, é só abrir e imprimir.
![Relatório final gerado](https://i.imgur.com/99yimUH.png)

---

### Requisitos de sistema

- Python3
