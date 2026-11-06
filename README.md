# IA Generativa no Ensino de Geociências

Manual vivo para docentes de geociências sobre o uso de IA generativa: atividades em sala, uso no trabalho docente e na pesquisa, e políticas de uso nas disciplinas.

**Leia online:** https://cdviana.github.io/iag-geociencias/
**Fichas do estudante:** https://cdviana.github.io/iag-geociencias/estudante/

<!-- Badge do DOI (Zenodo) após a primeira release -->

## Estrutura

```
\_quarto.yml               configuração comum (título, tema, formatos)
\_quarto-docente.yml       lista de capítulos do livro completo (perfil padrão)
\_quarto-estudante.yml     lista de capítulos das Fichas do Estudante
index.qmd                 apresentação
fundamentos/              Parte I
docente/                  Parte II  — IAG no trabalho docente
politicas/                Parte III — níveis, modelo de política, declaração
atividades/               Parte IV  — atividades + \_modelo-atividade.qmd
avaliacao/                Parte V
critica/                  Parte VI
apendices/                curadoria, prompts, ferramentas, glossário, contribuição
referencias.bib           fonte única de referências
styles/blocos.css         estilo dos blocos Para ir além / Armadilha / Na prática
.github/                  publicação automática e modelos de issue
```

## Publicar pela primeira vez

1. Crie um repositório público no GitHub chamado `iag-geociencias` e envie estes arquivos para a branch `main`.
2. Em **Settings → Pages → Build and deployment → Source**, escolha **GitHub Actions**.
3. Em `\_quarto.yml`, troque `SEU-USUARIO` pelo seu usuário ou organização. Faça o mesmo neste README.
4. Faça um *push*. A aba **Actions** mostra a renderização; em poucos minutos o livro estará no endereço acima.

## Trabalhar localmente

Instale o [Quarto](https://quarto.org/docs/get-started/) e, na pasta do repositório:

```bash
quarto preview                      # pré-visualização com recarga automática
quarto render                       # versão do docente  → \_book/
quarto render --profile estudante   # fichas do estudante → \_book/estudante/
```

Para gerar PDF localmente, instale também o TinyTeX: `quarto install tinytex`.

## Versões citáveis (DOI)

1. Conecte o repositório ao [Zenodo](https://zenodo.org) (Account → GitHub → ativar o repositório).
2. Crie uma *release* no GitHub (ex.: `v0.1.0`). O Zenodo gera um DOI para cada release e um DOI conceitual para todas as versões.
3. Atualize `CITATION.cff` e o badge acima.

## Licenças

* Texto: [CC BY 4.0](LICENSE.md)
* Código e prompts: [MIT](LICENSE-CODE)

## Contribuir

Veja [CONTRIBUTING.md](CONTRIBUTING.md).

