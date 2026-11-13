

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
