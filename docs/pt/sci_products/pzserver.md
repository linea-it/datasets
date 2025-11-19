# Dados do Photo-z Server

!!! Warning "Aviso"
    Página em construção. Parte do conteúdo pode estar incompleto.

O Photo-z Server (Servidor de Photo-z) é uma plataforma web desenvolvida pelo LIneA como parte da contribuição in-kind do Brasil para o projeto LSST do Observatório Rubin.

Os administradores do Photo-z Server mantêm e atualizam periodicamente uma lista curada de recursos de dados para apoiar a Comunidade LSST com produtos de dados relacionados a photo-z. Esta página fornece uma visão geral de alguns conjuntos de dados disponíveis no Photo-z Server juntamente com instruções de acesso. Para mais detalhes sobre os recursos e funcionalidades da plataforma, consulte a [**Documentação Completa do Photo-z Server para Usuários**](https://docs.linea.org.br/sci-platforms/pz_server.html).


!!! info "Acesso Restrito"
    De acordo com as Políticas de Dados do Observatório Rubin e do IDAC-BR, o acesso aos dados do LSST — incluindo produtos derivados hospedados no Photo-z Server — é restrito a membros autorizados da Comunidade LSST com contas RSP válidas.


## Classificação dos Conjuntos de Dados   

<font size=4> Conjuntos de Dados Oficiais </font><br>

Os conjuntos de dados oficiais serão produzidos pela equipe de Gerenciamento de Dados do Rubin e estarão disponíveis para a Comunidade LSST através do Photo-z Server. Esses conjuntos de dados incluirão catálogos de redshift de referência, conjuntos de treinamento e estimativas de photo-z associadas aos lançamentos de dados do LSST. Os conjuntos de dados serão lançados de forma escalonada, começando com o primeiro lançamento de dados (DR1) e continuando com lançamentos subsequentes conforme o progresso do levantamento LSST.

Por enquanto, a página de [Produtos de Dados Oficiais do Observatório Rubin](https://pzserver.linea.org.br/oficial_products) está vazia.

<font size=4> Conjuntos de Dados Não Oficiais </font><br>

Além dos dados carregados por usuários, a página de [Produtos de Dados Gerados por Usuários](https://pzserver.linea.org.br/user_products) hospeda conjuntos de dados que foram preparados pela equipe do LIneA para fins educacionais, para servir como exemplos de casos de uso para os tutoriais do Photo-z Server. Além disso, os conjuntos de dados DP1 gerados pela Unidade de Ciência de PZ da Equipe de Comissionamento do Rubin, descritos na nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/), também estão disponíveis lá. Todos esses conjuntos de dados não são classificados como Conjuntos de Dados Oficiais.

--- 


## Data Preview 1 


!!! warning "ATENÇÃO: Conjuntos de Dados Preliminares"  
    Esses conjuntos de dados foram produzidos pela Unidade de Ciência de PZ — um grupo de trabalho da Equipe de Comissionamento do Rubin — durante os _Estudos iniciais de redshifts fotométricos com LSSTComCam a partir do DP1_. Todos os resultados, juntamente com descrições detalhadas dos conjuntos de dados, estão disponíveis na nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/).

    **Esses conjuntos de dados NÃO são classificados como Conjuntos de Dados Oficiais lançados pela equipe de DM do Rubin.**  



Os conjuntos de dados descritos na nota técnica estão disponíveis no [Photo-z Server](https://pzserver.linea.org.br) como produtos de dados com o sufixo `SITCOMTN-154`. Seus links e breves descrições estão organizados por tipos de produtos abaixo.


### Catálogos de Objetos 


Produtos de dados contendo tabelas de objetos descritas na Seção 2.1 e listadas na Tabela 1 da nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/).


| Produto de Dados                 | Conjunto de Dados        | Seleção    | Número de Objetos | 
|----------------------------------|--------------------------|------------|-------------------|
| DP1 (disponível no RSP)          | Catálogo de Objetos Completo DP1| Nenhuma | 2.299.757 |  
|[ECDFS+EDFS+SV_95 gold SITCOMTN-154](https://pzserver.linea.org.br/product/78_ecdfsedfssv_95_gold_sitcomtn154) | ECDFS+EDFS+SV_95|gold|375.610|  
|[SV_38 gold_4_band SITCOMTN-154](https://pzserver.linea.org.br/product/79_sv_38_gold_4_band_sitcomtn154)| SV_38|gold_4_band|169.034| 

 
Conjunto de dados Gold abrangente de todos os campos DP1 além dos campos ECDFS+EDFS+SV_95 e SV_38, onde dados espectroscópicos estão disponíveis (conjunto de dados **não** listado na Tabela 1 da nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/)):   


| Produto de Dados                 | Conjunto de Dados        | Seleção   | Número de Objetos | 
|----------------------------------|--------------------------|-----------|-------------------|
|[DP1 Gold all](https://pzserver.linea.org.br/product/80_dp1_gold_all_sitcomtn154)| Todos os campos | gold | 686.334|
   




### Catálogos de Redshift de Referência 

#### Catálogos de Redshift de Referência de Levantamentos Individuais 

Produtos de dados contendo catálogos de redshifts de referência (antes do cruzamento com a tabela de Objetos DP1) separados pela pesquisa de origem, conforme listados na Tabela 2 da nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/).

**Nota:** Esses conjuntos de dados já foram filtrados para o campo ECDFS e limpos com os critérios de seleção descritos na Seção 2.2.1 da nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/). Para os catálogos originais completos, consulte a seção [Conjuntos de Dados Externos](#conjuntos-de-dados-externos) abaixo.

| Produto de Dados | Referência | Número de Redshifts |
|------------------|-----------|---------------------|
| [2dFGRS SITCOMTN-154](https://pzserver.linea.org.br/product/60_2dfgrs_sitcomtn154) | [Colless et al. (2001)](https://ui.adsabs.harvard.edu/abs/2001MNRAS.328.1039C) | 278 |
| [2dflens SITCOMTN-154](https://pzserver.linea.org.br/product/61_2dflens_sitcomtn154) | [Blake et al. (2016)](https://ui.adsabs.harvard.edu/abs/2016MNRAS.462.4240B) | 1 |
| [2MRS SITCOMTN-154](https://pzserver.linea.org.br/product/62_2mrs_sitcomtn154) | [Huchra et al. (2012)](https://ui.adsabs.harvard.edu/abs/2012ApJS..199...26H) | 9 |
| [3D-HST SITCOMTN-154](https://pzserver.linea.org.br/product/63_3dhst_sitcomtn154) | [Momcheva et al. (2016)](https://ui.adsabs.harvard.edu/abs/2016ApJS..225...27M) | 4237 |
| [6dFGS SITCOMTN-154](https://pzserver.linea.org.br/product/64_6dfgs_sitcomtn154) | [Jones et al. (2009)](https://ui.adsabs.harvard.edu/abs/2009MNRAS.399..683J) | 5 |
| [astrodeep SITCOMTN-154](https://pzserver.linea.org.br/product/65_astrodeep_sitcomtn154) | [Merlin et al. (2021)](https://ui.adsabs.harvard.edu/abs/2021A&A...649A..22M) | 35108 |
| [astrodeep_jwst SITCOMTN-154](https://pzserver.linea.org.br/product/66_astrodeep_jwst_sitcomtn154) | [Merlin et al. (2024)](https://ui.adsabs.harvard.edu/abs/2024A&A...691A.240M) | 76748 |
| [CANDELS SITCOMTN-154](https://pzserver.linea.org.br/product/67_candels_sitcomtn154) | [Kodra et al. (2023)](https://ui.adsabs.harvard.edu/abs/2023ApJ...942...36K) | 31440 |
| [JADES SITCOMTN-154](https://pzserver.linea.org.br/product/68_jades_sitcomtn154) | [D'Eugenio et al. (2025)](https://ui.adsabs.harvard.edu/abs/2025ApJS..277....4D) | 1224 |
| [MOSDEF SITCOMTN-154](https://pzserver.linea.org.br/product/69_mosdef_sitcomtn154) | [Kriek et al. (2015)](https://ui.adsabs.harvard.edu/abs/2015ApJS..218...15K) | 51 |
| [NED SITCOMTN-154](https://pzserver.linea.org.br/product/70_ned_sitcomtn154) | [Helou et al. (1991)](https://ui.adsabs.harvard.edu/abs/1991ASSL..171...89H) | 3770 |
| [OzDES SITCOMTN-154](https://pzserver.linea.org.br/product/71_ozdes_sitcomtn154) | [Lidman et al. (2020)](https://ui.adsabs.harvard.edu/abs/2020MNRAS.496...19L) | 1147 |
| [PRIMUS SITCOMTN-154](https://pzserver.linea.org.br/product/72_primus_sitcomtn154) | [Cool et al. (2013)](https://ui.adsabs.harvard.edu/abs/2013ApJ...767..118C) | 7352 |
| [VANDELS SITCOMTN-154](https://pzserver.linea.org.br/product/73_vandels_sitcomtn154) | [Garilli et al. (2021)](https://ui.adsabs.harvard.edu/abs/2021A&A...647A.150G) | 450 |
| [VIMOS SITCOMTN-154](https://pzserver.linea.org.br/product/74_vimos_sitcomtn154) | [Balestra et al. (2010)](https://ui.adsabs.harvard.edu/abs/2010A&A...512A..12B) | 1578 |
| [VUDS SITCOMTN-154](https://pzserver.linea.org.br/product/75_vuds_sitcomtn154) | [Tasca et al. (2017)](https://ui.adsabs.harvard.edu/abs/2017A&A...600A.110T) | 160 |
| [VVDS SITCOMTN-154](https://pzserver.linea.org.br/product/76_vvds_sitcomtn154) | [Le Fèvre et al. (2005)](https://ui.adsabs.harvard.edu/abs/2005A&A...439..845L) | 669 |



Dados espectroscópicos adicionais do DESI DR1 foram usados como um conjunto de teste independente para validação das estimativas de photo-z. Como o DESI DR1 é um conjunto de dados muito grande que se estende além da área de cobertura do DP1, foi filtrado para incluir apenas o campo ECDFS.


| Produto de Dados | Referência       | Número de Redshifts | 
|------------------|------------------|----------------------|
| [DESI DR1 inside DP1](https://pzserver.linea.org.br/product/34_desi_dr1_inside_dp1)| [DESI Collaboration et al. (2025)](https://arxiv.org/abs/2503.14745) |50.634 |



#### Catálogo de Redshift Combinado

Um único arquivo contendo todos os redshifts de referência combinados dos levantamentos individuais listados acima (excluindo DESI), conforme descrito na Seção 2.2.1 da nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/).

| Produto de Dados | Número de Redshifts |
|------------------|---------------------|
| [ComCam ECDFS z catalog SITCOMTN-154](https://pzserver.linea.org.br/product/77_comcam_ecdfs_z_catalog_sitcomtn154) |104.070| 









### Conjuntos de Treinamento e Teste 

No Photo-z Server, o tipo de produto "Training Set" abrange todas as amostras resultantes do cruzamento entre um redshift de referência e um catálogo de objetos. Isso pode incluir conjuntos de treinamento e teste juntos em um mesmo arquivo ou subamostras independentes carregadas separadamente. Para este último, tanto os conjuntos de treinamento quanto os de teste são marcados como "Training Set".


Produtos de dados contendo conjuntos de treinamento e teste gerados a partir do catálogo ComCam ECDFS z listados na Tabela 1 da nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/) são:


| Produto de Dados                 | Conjunto de Dados        | Seleção    | Número de Objetos | 
|----------------------------------|--------------------------|------------|-------------------|
| [training_v1 match_prelim SITCOMTN-154](https://pzserver.linea.org.br/product/81_training_v1_match_prelim_sitcomtn154) | training_v1 | match_prelim | 7.000 |
| [test_v1 match_prelim SITCOMTN-154](https://pzserver.linea.org.br/product/82_test_v1_match_prelim_sitcomtn154)         | test_v1     | match_prelim | 2.437 | 
| [training_v4 match_ecdfs SITCOMTN-154](https://pzserver.linea.org.br/product/83_training_v4_match_ecdfs_sitcomtn154)  | training_v4 | match_ecdfs  | 6.778 |
| [test_v4 match_ecdfs SITCOMTN-154](https://pzserver.linea.org.br/product/84_test_v4_match_ecdfs_sitcomtn154)          | test_v4     | match_ecdfs  | 2.905 |      
| [test_DESI match_desi SITCOMTN-154](https://pzserver.linea.org.br/product/85_test_desi_match_desi_sitcomtn154)        | test_DESI   | match_desi   | 2.728 |    



### Resultados de Treinamento 

Modelos de dados de estimadores listados na Tabela 7 e descritos no Apêndice A.3 da nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/).


| Gold baseline | Gold DP1 optimize | Gold DP1 optimize 4band |  
|---------------|-------------------|--------------------------| 
| [BPZ model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/90_bpz_model_gold_baseline_sitcomtn154)        | [BPZ model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/97_bpz_model_gold_dp1_optimize_sitcomtn154)        | [BPZ model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/105_bpz_model_gold_dp1_optimize_4band_sitcomtn154)        | 
| [CMNN model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/91_cmnn_model_gold_baseline_sitcomtn154)      | [CMNN model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/98_cmnn_model_gold_dp1_optimize_sitcomtn154)      | [CMNN model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/106_cmnn_model_gold_dp1_optimize_4band_sitcomtn154)      | 
| [DNF model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/92_dnf_model_gold_baseline_sitcomtn154)        | [DNF model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/99_dnf_model_gold_dp1_optimize_sitcomtn154)        | [DNF model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/107_dnf_model_gold_dp1_optimize_4band_sitcomtn154)        | 
| [FlexZBoost model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/93_flexzboost_model_gold_baseline_sitcomtn154) | [FlexZBoost model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/100_flexzboost_model_gold_dp1_optimize_sitcomtn154) | [FlexZBoost model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/108_flexzboost_model_gold_dp1_optimize_4band_sitcomtn154) | 
| [GPz model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/94_gpz_model_gold_baseline_sitcomtn154)        | [GPz model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/101_gpz_model_gold_dp1_optimize_sitcomtn154)        | [GPz model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/109_gpz_model_gold_dp1_optimize_4band_sitcomtn154)        | 
| [kNN model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/95_knn_model_gold_baseline_sitcomtn154)        | [kNN model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/102_knn_model_gold_dp1_optimize_sitcomtn154)        | [kNN model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/110_knn_model_gold_dp1_optimize_4band_sitcomtn154)        | 
| N/A                                              | [LePhare model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/103_lephare_model_gold_dp1_optimize_sitcomtn154) | [LePhare model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/111_lephare_model_gold_dp1_optimize_4band_sitcomtn154) | 
| [TPZ model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/96_tpz_model_gold_baseline_sitcomtn154)        | [TPZ model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/104_tpz_model_gold_dp1_optimize_sitcomtn154)        | [TPZ model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/112_tpz_model_gold_dp1_optimize_4band_sitcomtn154)        | 



<font size=4> Arquivos de Configuração </font><br>
 
Conforme mencionado na Seção 3.4 e Apêndice A.1 da nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/), os arquivos de configuração [dp1.yaml](https://github.com/LSSTDESC/rail_project_config/blob/main/dp1/dp1.yaml) (conjunto completo de configurações testadas, rotuladas como _flavors_ de análise) e [dp1_v4.yaml](https://github.com/LSSTDESC/rail_project_config/blob/main/dp1/dp1_v4.yaml) (parâmetros de configuração otimizados) estão disponíveis no repositório GitHub [`rail_project_config`](https://github.com/LSSTDESC/rail_project_config).
 

### Resultados de Validação 

Estimativas pontuais de photo-z, QP Ensembles e métricas de avaliação relacionadas aos resultados mostrados na Tabela 4. Arquivos carregados dos diretórios listados na Tabela 7 e descritos no Apêndice A.4 da nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/).




| Gold baseline | Gold DP1 optimize | Gold DP1 optimize  4band | 
|---|---|:-:| 
| [BPZ test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/113_bpz_test_gold_baseline_sitcomtn154)               | [BPZ test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/120_bpz_test_gold_dp1_optimize_sitcomtn154)               | :material-hammer-wrench: |
| [CMNN test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/114_cmnn_test_gold_baseline_sitcomtn154)             | [CMNN test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/121_cmnn_test_gold_dp1_optimize_sitcomtn154)             | :material-hammer-wrench: |
| [DNF test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/115_dnf_test_gold_baseline_sitcomtn154)               | [DNF test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/122_dnf_test_gold_dp1_optimize_sitcomtn154)               | :material-hammer-wrench: |
| [FlexZBoost test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/116_flexzboost_test_gold_baseline_sitcomtn154) | [FlexZBoost test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/123_flexzboost_test_gold_dp1_optimize_sitcomtn154) | :material-hammer-wrench: |
| [GPz test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/117_gpz_test_gold_baseline_sitcomtn154)               | [GPz test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/124_gpz_test_gold_dp1_optimize_sitcomtn154)               | :material-hammer-wrench: |
| [kNN test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/118_knn_test_gold_baseline_sitcomtn154)               | [kNN test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/125_knn_test_gold_dp1_optimize_sitcomtn154)               | :material-hammer-wrench: |
| N/A   | [LePhare test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/126_lephare_test_gold_dp1_optimize_sitcomtn154)       | :material-hammer-wrench: |
| [TPZ test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/119_tpz_test_gold_baseline_sitcomtn154)               | [TPZ test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/127_tpz_test_gold_dp1_optimize_sitcomtn154)               | :material-hammer-wrench: |


**Legenda**<br>
:material-hammer-wrench: Em preparação




### Estimativas de Photo-z 

#### Tabelas de Photo-z 

Tabelas de PZ produzidas como parte dos estudos iniciais com dados de comissionamento descritos em [SITCOMTN-154](https://sitcomtn-154.lsst.io/). Dados carregados dos diretórios listados na Tabela 7.


| Produto de Dados  | Número de Objetos |
|-------------------|-------------------|
| [PZ table dp1_all gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/128_pz_table_dp1_all_gold_baseline_sitcomtn154) | 686.334  | 
| [PZ table dp1_sv38 gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/129_pz_table_dp1_sv38_gold_baseline_sitcomtn154) | 169.034  | 
|[PZ table DESI gold baseline](https://pzserver.linea.org.br/product/130_pz_table_desi_gold_baseline_sitcomtn154) | 2728  |
| PZ table dp1_all gold dp1_optimize | :material-hammer-wrench: <!--375,610-->  | 
| PZ table dp1_sv_38 gold dp1_optimize | :material-hammer-wrench:  | 
| PZ table dp1_all gold dp1_optimize 4band | :material-hammer-wrench:  | 
| PZ table dp1_sv_38 gold dp1_optimize 4band | :material-hammer-wrench:  | 

**Legenda**<br>
:material-hammer-wrench: Em preparação




--- 

## Conjuntos de Dados Externos 

Dados públicos coletados da literatura e hospedados no Photo-z Server.


### Catálogos de Redshift de Referência 

#### Levantamentos Individuais

O PZ Server hospeda vários catálogos públicos de redshifts espectroscópicos de diferentes levantamentos que podem ser usados como conjuntos de dados de referência para treinamento e validação de estimativas de photo-z. Os produtos de dados listados abaixo são os catálogos originais, sem qualquer filtro ou seleção de dados.

| Produto de Dados | Referência | Número de Redshifts | Status |
|------------------|-----------|---------------------|---| 
| [2dFGRS Final Data Release](https://pzserver.linea.org.br/product/170_2dfgrs_final_data_release) | [Colless et al. (2001)](https://ui.adsabs.harvard.edu/abs/2001MNRAS.328.1039C) | 245,591 | :material-check:  | 
| [2dFLens Final Data Release](https://pzserver.linea.org.br/product/171_2dflens_final_data_release) | [Blake et al. (2016)](https://ui.adsabs.harvard.edu/abs/2016MNRAS.462.4240B) | 70,079 | :material-check:  | 
| [2MRS v240](https://pzserver.linea.org.br/product/172_2mrs_v240) | [Huchra et al. (2012)](https://ui.adsabs.harvard.edu/abs/2012ApJS..199...26H) | 240,496 | :material-check:  | 
| [3D-HST v415](https://pzserver.linea.org.br/product/173_3dhst_v415) | [Momcheva et al. (2016)](https://ui.adsabs.harvard.edu/abs/2016ApJS..225...27M) | 207,967 | :material-check:  | 
| [6dFGS DR3](https://pzserver.linea.org.br/product/174_6dfgs_dr3) | [Jones et al. (2009)](https://ui.adsabs.harvard.edu/abs/2009MNRAS.399..683J) | 136,304 | :material-check:  | 
| ACES | - | - | :material-clock-outline: | 
| ATLAS | - | - | :material-clock-outline: | 
| [ASTRODEEP GS43](https://pzserver.linea.org.br/product/176_astrodeep_gs43) | [Merlin et al. (2021)](https://ui.adsabs.harvard.edu/abs/2021A&A...649A..22M/abstract) | 35,108 | :material-check:  | 
| [ASTRODEEP JWST](https://pzserver.linea.org.br/product/177_astrodeep_jwst) | [Merlin et al. (2024)](https://ui.adsabs.harvard.edu/abs/2024A%26A...691A.240M/abstract) | 531,173 | :material-check:  | 
| C3R2 DR3 | - | - | :material-clock-outline: | 
| CANUCS SMACS | - | - | :material-clock-outline: | 
| CDB | - | - | :material-clock-outline: | 
| CLASH-VLT FR | - | - | :material-clock-outline: | 
| COSMOS 2025 | - | - | :material-clock-outline: | 
| DEEP2 DR4 | - | - | :material-clock-outline: | 
| DEIMOS 10K | - | - | :material-clock-outline: | 
| DESI EDR | [DESI Collaboration et al. (2025)](https://arxiv.org/abs/2503.14745) | 2.451.325 |  :material-hammer-wrench:  | 
| [DESI DR1 within LSST DP1](https://pzserver.linea.org.br/product/178_desi_dr1_within_lsst_dp1) | [DESI Collaboration et al. (2025)](https://ui.adsabs.harvard.edu/abs/2025arXiv250314745D/abstract) | 50,634 | :material-check:  | 
| Euclid Q1 SPE | - | - | :material-clock-outline: |
| FMOS-COSMOS | - | - | :material-clock-outline: |
| AMA DR4 | - | - | :material-clock-outline: |
| GLASS | - | - | :material-clock-outline: |
| HectoMAP DR2 | - | - | :material-clock-outline: |
| HETDEX DR1 | - | - | :material-clock-outline: |
| [JADES DR3](https://pzserver.linea.org.br/product/179_jades_dr3) | [D'Eugenio et al. (2025)](https://ui.adsabs.harvard.edu/abs/2025ApJS..277....4D/abstract) | 8,172 | :material-check:  | 
| LEGA-C DR3 |  - | - | :material-clock-outline: |
| MOSDEF (MOSFIRE) FR |  - | - | :material-clock-outline: |
| MUSE DR1 | - | - | :material-clock-outline: |
| OzDES DR2 | [Lidman et al. (2020)](https://ui.adsabs.harvard.edu/abs/2020MNRAS.496...19L) | 38.624 |:material-hammer-wrench:  | 
| PRIMUS DR1| [Cool et al. (2013)](https://ui.adsabs.harvard.edu/abs/2013ApJ...767..118C) | 213.696 |:material-hammer-wrench:  | 
| SAGA DR2 | - |  | :material-clock-outline: |
| SDSS DR17 | - |  | :material-clock-outline: |
| SpARCS | - |  | :material-clock-outline: |
| SPT-GMOS | - |  | :material-clock-outline: |
| UDS | - |  | :material-clock-outline: |
| VANDELS DR4 | [Garilli et al. (2021)](https://ui.adsabs.harvard.edu/abs/2021A&A...647A.150G) | 2.165 |:material-hammer-wrench:  | 
| VIPERS | - | -  | :material-clock-outline: |
| VLT-VIMOS v201 | [Balestra et al. (2010)](https://ui.adsabs.harvard.edu/abs/2010A&A...512A..12B) | 5.052 |:material-hammer-wrench:  | 
| VUDS |  - | -  | :material-clock-outline: |
| VVDS Final Data Release | [Le Fèvre et al. (2005)](https://ui.adsabs.harvard.edu/abs/2005A&A...439..845L) | 40.944 |:material-hammer-wrench:  | 
| WiggleZ | - | -  | :material-clock-outline: | 
| zCOSMOS 20k/10k | - | -  | :material-clock-outline: | 
| ZFIRE | - | -  | :material-clock-outline: | 


**Legenda**<br>
:material-clock-outline: Planejado &emsp; :material-hammer-wrench: Em preparação &emsp; :material-check: Disponível 



#### Catálogos Combinados


| Produto de Dados | Data de Lançamento | # de Levantamentos | # de Redshifts | Status | 
|------------------|--------------------|--------------------|----------------|---     |  
| Todos os redshifts combinados | Nov 2025 |   -  | -  | :material-hammer-wrench:  | 
| Redshifts combinados na área de cobertura DP1 | Nov 2025 |    -  | -   |  :material-hammer-wrench:  |          


**Legenda**<br>
:material-clock-outline: Planejado &emsp; :material-hammer-wrench: Em preparação &emsp; :material-check: Disponível 

<!--
Acesso rápido via biblioteca `pzserver`: 

```python
pz_server.get_product('<dataset_name>') 
``` 
-->


### Conjuntos de Treinamento   

O resultado do cruzamento espacial entre as compilações de redshift e os dados fotométricos do LSST.   

| Produto de Dados | Data de Lançamento | # de Galáxias | Status | 
|------------------|--------------------|--------------  |---     |
| DP1 matched  | Nov 2025     |   -           | :material-hammer-wrench:  | 


**Legenda**<br>
:material-clock-outline: Planejado &emsp; :material-hammer-wrench: Em preparação &emsp; :material-check: Disponível 


<!--
Acesso rápido via biblioteca `pzserver`: 

```python
pz_server.get_product('<dataset_name>') 
``` 

--> 




