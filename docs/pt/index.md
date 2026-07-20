# Dados

Bem-vindo à página de documentação de dados do LIneA. Aqui você encontra informações sobre os conjuntos de dados disponíveis e orientações para acessá-los.


### Perfis de usuário e níveis de acesso 
O LIneA oferece diferentes perfis de usuário, cada um com níveis de acesso específicos aos dados e serviços disponíveis. 
Para saber quais serviços estão disponíveis para cada perfil, consulte a [tabela](https://docs.linea.org.br/sci-platforms/index.html#acesso-aos-servicos-e-plataformas-linea) disponível na página de informações sobre as plataformas científicas no site de [documentação para usuários](https://docs.linea.org.br). 


---

## Catálogos

O acesso a dados tabulares (catálogos) é realizado por meio de diferentes aplicações do [LIneA Science Platform (LSP)](https://scienceplatform.linea.org.br/lsp), conforme o tamanho, o tipo ou os níveis de permissão de acesso estabelecidos pelo levantamento astronômico de origem.

Para navegar, utilize o menu à esquerda e explore os diferentes conjuntos de dados, organizados de acordo com as opções de uso:

- **Download** e **acesso programático** com [LSDB](https://lsdb.io/) (dados no formato [HATS](https://hats.readthedocs.io/en/latest/))
- **Consulta** em banco de dados, por meio das plataformas [User Query](https://userquery.linea.org.br/), [Jupyter Hub](https://jupyter.linea.org.br/) ou [TAP Service](https://userquery.linea.org.br/cms/services/scripted-access/)
- **Processamento** no ambiente HPC de dados armazenados no sistema Lustre, com acesso pela plataforma [Open OnDemand](https://ondemand.linea.org.br)
- **Visualização** de informações de catálogos sobrepostas a imagens [HiPS](https://aladin.cds.unistra.fr/hips/)

Confira abaixo a tabela com o resumo dos principais catálogos disponíveis para download ou consulta por meio dos diferentes serviços:

| Survey / release      | LSDB                     | Banco de dados           | HPC                      | HiPS Catalog             |
|-----------------------|--------------------------|--------------------------|--------------------------|--------------------------|
| 2MASS PSC             | :material-account-group: | :material-account-group: | :material-lock:          | :material-account-group: |
| COSMO DC2             | -                        | -                        | :material-lock:          | -                        |
| DELVE DR2             | :material-account-group: | -                        | :material-lock:          | -                        |
| DES DR2 Main          | :material-account-group: | :material-account-group: | :material-lock:          | :material-account-group: |
| DES DR2 Y6 Gold       | :material-account-group: | :material-account-group: | :material-lock:          | :material-hammer-wrench: |
| DESI DR1              | :material-account-group: | -                        | :material-lock:          | -                        |
| eRASS1 Main           | :material-account-group: | -                        | :material-lock:          | -                        |
| Euclid Q1             | :material-account-group: | -                        | :material-lock:          | -                        |
| Gaia DR3 Source       | :material-account-group: | :material-account-group: | :material-lock:          | -                        |
| GALEX                 | :material-account-group: | -                        | :material-lock:          | :material-account-group: |
| HSC                   | :material-account-group: | -                        | :material-lock:          | -                        |
| LSST DP0.1            | -                        | -                        | :material-lock:          | -                        |
| LSST DP0.2            | -                        | :material-lock:          | :material-lock:          | -                        |
| LSST DP1              | :material-lock:          | :material-lock:          | :material-lock:          | :material-lock:          |
| LSST DP2              | :material-hammer-wrench: | :material-hammer-wrench: | :material-hammer-wrench: | :material-hammer-wrench: |
| LSST DR1-DR11         | :material-clock-outline: | :material-clock-outline: | :material-clock-outline: | :material-clock-outline: |
| MPC                   | -                        | :material-account-group: | -                        | -                        |
| Pan-STARRS            | :material-account-group: | -                        | :material-lock:          | -                        |
| S-PLUS                | :material-clock-outline: | -                        | :material-clock-outline: | -                        |
| SDSS DR7              | :material-account-group: | -                        | :material-lock:          | -                        |
| SkyMapper             | :material-account-group: | -                        | :material-lock:          | -                        |
| TESS                  | :material-account-group: | -                        | :material-lock:          | -                        |
| TNS                   | :material-account-group: | -                        | :material-lock:          | -                        |
| VSX                   | :material-account-group: | -                        | :material-lock:          | -                        |
| WISE                  | :material-account-group: | -                        | :material-lock:          | -                        |
| ZTF                   | :material-account-group: | -                        | :material-lock:          | -                        |

**Legenda**<br>
:material-account-group: Público &emsp; :material-lock: Acesso restrito &emsp; :material-clock-outline: Planejado &emsp; :material-hammer-wrench: Em preparação

---

## Imagens

O acesso às imagens astronômicas é realizado por meio de diferentes aplicações do LIneA Science Platform, conforme o tipo de imagem e o levantamento astronômico de origem.

- Imagens [HiPS](https://aladin.cds.unistra.fr/hips/) (Hierarchical Progressive Surveys): **visualização global** e **navegação** pela aplicação [Sky Viewer](https://skyviewer.org/), ou para apontar para uma lista de alvos previamente selecionados no [Target Viewer](https://targetviewer.linea.org.br/).

- Imagens [FITS](https://fits.gsfc.nasa.gov/) (Flexible Image Transport System) coadicionadas: **download** de cutouts pelo [Target Viewer](https://targetviewer.linea.org.br/), **acesso programático** via API pelo [Jupyter Hub](https://jupyter.linea.org.br/) ou **processamento** no ambiente HPC, com acesso pela plataforma [Open OnDemand](https://ondemand.linea.org.br).

- Imagens [FITS](https://fits.gsfc.nasa.gov/) (Flexible Image Transport System) de exposição única: **acesso programático** via API pelo [Jupyter Hub](https://jupyter.linea.org.br/) ou **processamento** no ambiente HPC, com acesso pela plataforma [Open OnDemand](https://ondemand.linea.org.br).

Confira abaixo a tabela com o resumo dos principais conjuntos de imagens disponíveis para download ou consulta por meio dos diferentes serviços:


| Survey / release            | HiPS                                      | FITS coadicionadas                        | FITS de exposição única              |
|-----------------------------|-------------------------------------------|-------------------------------------------|--------------------------------------|
| DES DR2                     | :material-account-group: :material-floppy:| :material-account-group: :material-floppy:| :material-lock: :material-floppy:    |
| Rubin First Look            | :material-account-group: :material-floppy:| -                                         | -                                    |
| LSST DP0.1                  | -                                         | :material-lock: :material-link:           | :material-lock: :material-link:      |
| LSST DP0.2                  | :material-lock: :material-floppy:         | :material-lock: :material-link:           | :material-lock: :material-link:      |
| LSST DP1                    | :material-lock: :material-floppy:         | :material-lock: :material-floppy:         | :material-lock: :material-link:      |
| LSST DP2                    | :material-clock-outline: :material-floppy:| :material-clock-outline: :material-floppy:| :material-clock-outline: :material-link:|
| LSST DR1-DR11               | :material-clock-outline: :material-floppy:| :material-clock-outline: :material-floppy:| :material-clock-outline: :material-link:|
| 2MASS colored               | :material-account-group: :material-link:  | -                                         | -                                    |
| AllWISE                     | :material-account-group: :material-link:  | -                                         | -                                    |
| DECaPS DR2                  | :material-account-group: :material-link:  | -                                         | -                                    |
| DSS Colored                 | :material-account-group: :material-link:  | -                                         | -                                    |
| DSS2 Red (F+R)              | :material-account-group: :material-link:  | -                                         | -                                    |
| Density Map Gaia EDR3       | :material-account-group: :material-link:  | -                                         | -                                    |
| Fermi Color                 | :material-account-group: :material-link:  | -                                         | -                                    |
| GALEXGR6_7 NUV              | :material-account-group: :material-link:  | -                                         | -                                    |
| GLIMPSE360                  | :material-account-group: :material-link:  | -                                         | -                                    |
| Halpha                      | :material-account-group: :material-link:  | -                                         | -                                    |
| IRAC color I1,I2,I4         | :material-account-group: :material-link:  | -                                         | -                                    |
| IRAC colored                | :material-account-group: :material-link:  | -                                         | -                                    |
| Mellinger colored           | :material-account-group: :material-link:  | -                                         | -                                    |
| PanSTARRS DR1 colored       | :material-account-group: :material-link:  | -                                         | -                                    |
| PanSTARRS DR1 g             | :material-account-group: :material-link:  | -                                         | -                                    |
| SDSS9 band-g                | :material-account-group: :material-link:  | -                                         | -                                    |
| SDSS9 colored               | :material-account-group: :material-link:  | -                                         | -                                    |
| VTSS-Ha                     | :material-account-group: :material-link:  | -                                         | -                                    |
| eROSITA-DE DR1 RGB          | :material-account-group: :material-link:  | -                                         | -                                    |


**Legenda**<br>
:material-account-group: Público &emsp; :material-lock: Acesso restrito &emsp; :material-clock-outline: Planejado &emsp; :material-hammer-wrench: Em preparação

:material-floppy: Cópia local &emsp; :material-link: Acesso remoto 


!!! abstract "Aviso"
    Esta é uma página de documentação em constante atualização. Algumas informações podem estar incompletas ou desatualizadas. Em caso de dúvidas, entre em contato com a equipe do LIneA através do e-mail: **[helpdesk@linea.org.br](mailto:helpdesk@linea.org.br)**. 

---

O LIneA - Laboratório Interinstitucional de e-Astronomia - é um laboratório multiusuário, operado por uma organização sem fins lucrativos (Associação LIneA) com apoio do Ministério da Ciência, Tecnologia e Inovação do Brasil.

Para saber mais, acesse [https://www.linea.org.br](https://www.linea.org.br).