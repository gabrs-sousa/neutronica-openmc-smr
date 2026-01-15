# Neutrônica com OpenMC — Estudo de SMRs

Este repositório reúne simulações e estudos em neutrônica realizados com o código **OpenMC**, com foco principal no **Reator Modular Pequeno (SMR) da Rolls-Royce**, sem boro solúvel, conforme descrito em _“Comparison of Advanced Technology Fuel Options in Soluble Boron-Free SMRs”_.

## Estrutura do Repositório

neutronica-openmc-smr/<br/>
├── 0_tutoriais/ # Exemplos e tutoriais adaptados (pin-cell, assemblies, etc)<br/>
├── 1_benchmark_rrsmr/ # Modelagem do RR-SMR (baseada no artigo de referência)<br/>
│ ├── geometry/<br/>
│ ├── materials/<br/>
│ ├── settings/<br/>
│ └── tallies/<br/>
├── 2_estudos_combustivel/ # Variações com ATFs (FeCrAl, U3Si2, revestimentos)<br/>
├── 3_pos_processamento/ # Scripts de pós-processamento e visualização (Jupyter)<br/>
└── README.md<br/>


## Requisitos

- Python 3.10+  
- OpenMC ≥ 0.13  
- Jupyter Notebooks  
- Bibliotecas: `matplotlib`, `numpy`, `openmc`, `pandas`  
- Dados ENDF/B-VIII.0 (HDF5) — [como baixar](https://docs.openmc.org/en/latest/usersguide/data.html)

## Como rodar

```bash
git clone https://github.com/seu-usuario/neutronica-openmc-smr.git
cd neutronica-openmc-smr
conda activate openmc-env
python3 main.py
```

## Referência principal

A. de Lara, X. Ha Nguyen, P. Van Uffelen, E. Shwageraus,<br/>
Comparison of Advanced Technology Fuel Options in Soluble Boron-Free SMRs,<br/>
Annals of Nuclear Energy, Volume 218, 2025, 111355, ISSN 0306-4549,<br/>
https://doi.org/10.1016/j.anucene.2025.111355.


## Observações

Todos os arquivos são de livre uso acadêmico sob a licença MIT.

Desenvolvido por Gabriel Sousa — mestrando em Engenharia Nuclear (IPEN/USP). <br/>
Contato: [LinkedIn](https://www.linkedin.com/in/gabrs-sousa/)