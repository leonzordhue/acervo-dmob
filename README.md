<!-- AKE/UFT-1.0 | BUILD: ACERVO-20260803 | IC: 1.0 | MÓDULO: ACERVO_DMOB -->
# Acervo DMOB — SEINFRA/AM

Acervo público do Departamento Rodoviário (DMOB): fotos de campo e traçados
KML/KMZ de rodovias, ramais e viários municipais do Amazonas. Consumido pelo
[seinfra-hub](https://leonzordhue.github.io/seinfra-hub/).

## Estrutura

| Pasta / arquivo | Conteúdo |
|---|---|
| `fotos/<rodovia>/<ramal>/` | Fotos de campo em resolução web (máx. 1600 px) |
| `thumbs/<rodovia>/<ramal>/` | Miniaturas (360 px) |
| `kml/1-rodovias/…` `2-ramais/…` `3-viarios/…` `4-colecoes/…` | Traçados KML/KMZ |
| `acervo_fotos.json` | Manifesto: pasta → rodovia, ramal, `ramal_key`, município, nº de fotos |
| `fotos_files.json` | Lista de arquivos por pasta (data e GPS de cada foto) |
| `acervo_kml.json` | Manifesto: arquivo → tipo, rodovia, ramal, `ramal_key`, URL |
| `galeria.html` | Galeria navegável ([abrir](https://leonzordhue.github.io/acervo-dmob/galeria.html)) |

## Correspondência com a plataforma

Cada item é casado com a base oficial de ramais por `ramal_key`
(= `CÓDIGO_Número`, ex.: `RMCRO_65`) — a mesma chave usada pelo hub.
A associação foto→ramal foi feita por GPS (foto a ≤150 m do traçado).

Resolução original das fotos e originais dos KML/KMZ: acervo interno do
departamento (`Acervo Visual` e `Acervo KML` no servidor de rede).

*Gerado e mantido pelo pipeline AKE/UFT-1.0 (DMOB).*
