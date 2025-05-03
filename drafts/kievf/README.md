# Dataset 'kievf'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/slav/aksl/kievfol/kievf.htm).

* URL: https://github.com/TITUS-2-0/slavonic/tree/main/drafts/kievf/
* version: unreleased
* date: 2025-04-09

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/slavonic/tree/main/drafts/kievf/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Folio | `div@folio` | Automatically translated into named div |
| Pagina | `div@pagina` | Automatically translated into named div |
| Line | `lb` |  |

### Structural overview
```text
text (@xml:lang=chu-Glag)
  body
    ab (@xml:id) (multiple)
      choice (multiple)
        reg (@type=transliteration) (multiple)
        orig (multiple)
      [lb (@n) (multiple)]
      [lb (@break=no, @n) (multiple)]
    [pb (@n) (multiple)]
```

### Structure Example

```xml
<pb xmlns="http://www.tei-c.org/ns/1.0" n="1v"/>
```
