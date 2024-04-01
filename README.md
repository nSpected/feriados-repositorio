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

## Obtendo Jsons do Repositório via HTTP GET:
### Observações:
- O .json no final da URL é obrigatório.

### Feriados Nacionais:
- ANO: Número representando o ano, atualmente (01/04/2024) apenas suporta 2024.
- PAÍS: Nome do país em snake_case, sem acentuação.
```
https://raw.githubusercontent.com/nSpected/feriados-repositorio/main/feriados/v1/ANO/PAÍS/nacionais.json
```

### Feriados Estaduais:
- ANO: Número representando o ano, atualmente (01/04/2024) apenas suporta 2024.
- PAÍS: Nome do país em snake_case, sem acentuação.
- ESTADO: Nome do estado em snake_case, sem acentuação.
```
https://raw.githubusercontent.com/nSpected/feriados-repositorio/main/feriados/v1/ANO/PAÍS/estaduais/ESTADO.json
```

### Feriados Municipais:
- ANO: Número representando o ano, atualmente (01/04/2024) apenas suporta 2024.
- PAÍS: Nome do país em snake_case, sem acentuação.
- ESTADO: Nome do estado em snake_case, sem acentuação.
- MUNICÍPIO: Nome do município em snake_case, sem acentuação.
```
https://raw.githubusercontent.com/nSpected/feriados-repositorio/main/feriados/v1/ANO/PAÍS/municipais/ESTADO/MUNICÍPIO.json
```
