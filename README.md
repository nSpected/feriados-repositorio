# Repositório de Feriados Brasileiros
Ainda em desenvolvimento... 🏗️🏗️🚧

# V1:

## Formato Json para Feriados:

### Campos:
- "data": Data do feriado, em formato americano (ano-mês-dia).
- "nome": Nome do feriado, quando não houver preencher com a palavra "Feriado" seguida do tipo, exemplo "Feriado Municipal".
- "tipoDeFeriado": Tipo do feriado, campo obrigatório que e case-sensitive, preencha com uma das seguintes opções:
- - "Nacional", "Estadual", ou "Municipal".
- "país": O nome do país ao qual o feriado se aplica, obrigatório.
- "unidadeFederativa": A sigla da unidade federativa ao qual o feriado se aplica, preencha apenas em feriados Estaduais e Municipais.
- "municipio": O nome do município ao qual o feriado se aplica, preencha apenas em feriados municipais.

### Exemplo:
```
[
    {
        "data": "2024-05-30",
        "nome": "Corpus Christi",
        "tipoDeFeriado": "Municipal",
        "país": "Brasil",
        "unidadeFederativa": "RS",
        "municipio": "Alvorada"
    }
]
```
