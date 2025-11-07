# Catálogos de Aglomerados WaZP DES Y6 Gold

!!! Warning "Aviso"
    Página em construção. Parte do conteúdo pode estar incompleto ou desatualizado.

## Visão Geral
Benoist et al. (2025) apresentam um catálogo de aglomerados de galáxias obtido pelo WaZP cluster finder, independente da detecção pela sequência vermelha, utilizando seis anos de dados do Dark Energy Survey (DES-Y6). O catálogo completo inclui mais de 400.000 aglomerados com Ngals > 5, alcançando redshifts de até z = 1,3. Uma versão homogenizada para uso em cosmologia contém 33.000 aglomerados ricos (Ngals > 25).

A comparação com o catálogo WaZP anterior, baseado nos dados do primeiro ano do DES (DES-Y1), mostra que praticamente todos os aglomerados dentro da área e profundidade sobrepostas são recuperados. Observações mais profundas do DES-Y6 e uma amostra espectroscópica mais completa melhoram as estimativas de redshift, resultando em um desvio médio de 1,4% e um offset médio de 0,2%.

Os aglomerados ópticos foram cruzados com amostras SZE dos telescópios SPT e ACT. Praticamente todos os aglomerados SZE em regiões sobrepostas possuem um correspondente no WaZP, e 90% dos aglomerados ópticos com riqueza > 150 têm equivalente nas regiões profundas das pesquisas SZE. Cerca de 15–20% dos sistemas SZE correspondentes apresentam múltiplos aglomerados WaZP dentro de R500c no mesmo redshift, sugerindo sistemas possivelmente em interação ou não relaxados. Os centramentos de aglomerados WaZP e SZE são consistentes quando se considera o tamanho dos feixes.

## Acesso aos Dados

- Catálogo de aglomerados: [y6a2_dnf_wazp_v5.0.12.6801_clusters.fits](https://datasets.linea.org.br/wazp/y6a2_dnf_wazp_v5.0.12.6801_clusters.fits)
- Membros dos aglomerados: [y6a2_dnf_wazp_v5.0.12.6801_members.fits](https://datasets.linea.org.br/wazp/y6a2_dnf_wazp_v5.0.12.6801_members.fits)
- Mapa da cobertura: [y6a2_dnf_wazp_v5.0.12.6801_footprint.fits](https://datasets.linea.org.br/wazp/y6a2_dnf_wazp_v5.0.12.6801_footprint.fits)

### Download com wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://datasets.linea.org.br/wazp/y6a2_dnf_wazp_v5.0.12.6801_clusters.fits
```

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://datasets.linea.org.br/wazp/y6a2_dnf_wazp_v5.0.12.6801_members.fits
```

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://datasets.linea.org.br/wazp/y6a2_dnf_wazp_v5.0.12.6801_footprint.fits
```


<div class="button-container">
<a href="https://des.ncsa.illinois.edu/releases/y6a2/Y6cluster-wazp" class="button-link">Descrição das Colunas</a>
<a href="https://arxiv.org/abs/2507.05360t" class="button-link">Artigo Científico</a>
</div>


