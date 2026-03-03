


O LIneA disponibiliza um acervo de catálogos de _redshifts_ espectroscópicos (spec-z) que foram publicamente distribuídos e detalhadamente descritos em literatura científica pelos seus projetos de origem. Estes catálogos foram coletados ao longo dos anos de operação do levantamento Dark Energy Survey (DES) e agrupados sistematicamente por uma ferramenta do DES Science Portal (_pipeline_ Spectroscopic Sample, [Gschwend et al., 2018](https://ui.adsabs.harvard.edu/abs/2018A%26C....25...58G/abstract)) para compor a base de um conjunto de treinamento para algoritmos de cálculo de _redshifts_ fotométricos baseados em aprendizado de máquina. A versão original do catálogo compilado utilizada no contexto do DES inclui dados proprietários do levantamento [OzDES](https://www.mso.anu.edu.au/ozdes/index.html) ([Yuan et al. 2015](https://ui.adsabs.harvard.edu/abs/2015MNRAS.452.3047Y/abstract)) e outros dados de pequenos levantamentos, também proprietários. 

Uma versão reduzida da amostra com ~3.6 milhões de _redshifts_ e o resultado da sua combinação com os dados fotométricos do DES DR2 estão temporariamente disponíveis para download no formato Parquet (vide comandos abaixo). 

Em breve, esta amostra será disponibilizada para os usuários do [**LIneA Science Platform**](https://scienceplatform.linea.org.br/lsp) com acesso através da interface [**User Query**](https://docs.linea.org.br/sci-platforms/user_query.html) ou programaticamente através do [**TAP Service**](https://docs.linea.org.br/sci-platforms/user_query.html#tap-service) e sofrerá atualizações regulares com a adição de dados de novos levantamentos.


## Catálogo compilado de _redshifts_ espectroscópicos públicos 

### Download 

```bash
$ wget -c https://datasets.linea.org.br/redshifts/public_specz_compilation.pq
```
### Caracterização 

A caracterização detalhada do catálogo compilado de _redshifts_ espectroscópicos públicos pode ser encontrada [neste notebook](https://datasets.linea.org.br/redshifts/public-specz-compilation.html). **Obs: o método de acesso aos dados utilizado no notebook está desatualizado, favor desconsiderá-lo.**    


## Conjunto de treinamento público para _redshifts_ fotométricos

### Download

```bash
$ wget -c https://datasets.linea.org.br/redshifts/public_pz_training_set.pq
```

### Caracterização

A caracterização detalhada do conjunto de treinamento público para _redshifts_ fotométricos pode ser encontrada [neste notebook](https://datasets.linea.org.br/redshifts/public-training-set-des-dr2.html). **Obs: o método de acesso aos dados utilizado no notebook está desatualizado, favor desconsiderá-lo.**
