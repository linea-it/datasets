LIneA pone a disposición un acervo de catálogos de *redshifts* espectroscópicos (spec-z) que han sido distribuidos públicamente y descritos detalladamente en la literatura científica por sus proyectos de origen. Estos catálogos fueron recopilados a lo largo de los años de operación del Dark Energy Survey (DES) y agrupados sistemáticamente mediante una herramienta del DES Science Portal (*pipeline* Spectroscopic Sample, [Gschwend et al., 2018](https://ui.adsabs.harvard.edu/abs/2018A%26C....25...58G/abstract)) para conformar la base de un conjunto de entrenamiento para algoritmos de estimación de *redshifts* fotométricos basados en aprendizaje automático. La versión original del catálogo compilado utilizada en el contexto del DES incluye datos propietarios del levantamiento OzDES ([Yuan et al. 2015](https://ui.adsabs.harvard.edu/abs/2015MNRAS.452.3047Y/abstract)) y otros datos propietarios de levantamientos más pequeños.

Una versión reducida de la muestra, con aproximadamente ~3,6 millones de *redshifts*, junto con el resultado de su combinación con los datos fotométricos del DES DR2, está temporalmente disponible para descarga en formato Parquet (véanse los comandos a continuación).

Próximamente, esta muestra estará disponible para los usuarios de la [**LIneA Science Platform**](https://scienceplatform.linea.org.br/lsp), con acceso a través de la interfaz [**User Query**](https://docs.linea.org.br/sci-platforms/user_query.html) o de manera programática mediante el [**TAP Service**](https://docs.linea.org.br/sci-platforms/user_query.html#tap-service), y será actualizada regularmente con la incorporación de datos de nuevos levantamientos.

## Catálogo compilado de *redshifts* espectroscópicos públicos

### Descarga

```bash
$ wget -c https://datasets.linea.org.br/redshifts/public_specz_compilation.pq
```

### Caracterización

La caracterización detallada del catálogo compilado de *redshifts* espectroscópicos públicos puede encontrarse en [este notebook](https://datasets.linea.org.br/redshifts/public-specz-compilation.html). **Nota: el método de acceso a los datos utilizado en el notebook está desactualizado; por favor, desconsidérelo.**

## Conjunto de entrenamiento público para *redshifts* fotométricos

### Descarga

```bash
$ wget -c https://datasets.linea.org.br/redshifts/public_pz_training_set.pq
```

### Caracterización

La caracterización detallada del conjunto de entrenamiento público para *redshifts* fotométricos puede encontrarse en [este notebook](https://datasets.linea.org.br/redshifts/public-training-set-des-dr2.html). **Nota: el método de acceso a los datos utilizado en el notebook está desactualizado; por favor, desconsidérelo.**
