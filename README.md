# Indicadores de orientação sexual, violência e parentalidade com dados da PNS em R

**[Acesse o site do minicurso para os materiais completos.](https://lincolntsilva.github.io/saude-sexualidade-pns-2019/)**

## Sobre o minicurso

Minicurso de 6 horas, em 2 encontros de 3 horas, sobre como construir, estimar e interpretar indicadores de orientação sexual, violência e parentalidade com os microdados da Pesquisa Nacional de Saúde (PNS) 2019 do IBGE, em um fluxo reprodutível com R e Quarto.

O curso usa o questionário do morador selecionado da PNS 2019, lido com o pacote `PNSIBGE`, e trata o desenho amostral com os pacotes `survey` e `srvyr`.

## Estrutura do repositório

| Arquivo | Conteúdo |
|---|---|
| `index.qmd` | Página inicial do site |
| `dia1.qmd`, `dia2.qmd` | Material de aula de cada dia |
| `relatorio.qmd` | Relatório final, parametrizado por recorte geográfico |
| `preparacao.qmd`, `dados.qmd`, `materiais.qmd`, `referencias.qmd`, `about.qmd` | Demais páginas do site |
| `_quarto.yml`, `tema.scss`, `styles.css` | Configuração e aparência do site |
| `_freeze/` | Resultados guardados dos cálculos, usados na publicação do site |

Os dados não ficam no repositório: a base do curso é gerada pelo próprio relatório, a partir dos microdados do IBGE, com o parâmetro `gerar_base: true`.

## Como gerar o site

Com R, Quarto e os pacotes do curso instalados (veja a página [Preparação](https://lincolntsilva.github.io/saude-sexualidade-pns-2019/preparacao.html)):

```bash
quarto render
```
