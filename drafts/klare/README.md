# Dataset 'Klaret, Grammar and Glossary'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/slav/acech/klaret/klare.htm).

* URL: https://github.com/TITUS-2-0/slavonic/tree/main/drafts/klare/
* version: unreleased
* date: 2025-03-10

## Citation
```text
Digital version of Klaret, Grammar and Glossary by Mg. Clareti de Solentia (draft version). By: Jost Gippert, Florian Matter, Petr Vavroušek. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/slavonic/tree/main/drafts/klare/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Part | `div@part` | Automatically translated into named div |
| Chapter | `div@chapter` | Automatically translated into named div |
| Line | `lb` |  |

### Structural overview
```text
text (@xml:lang=ces-Latn-x-old-czech)
  body
    div (@data-level=1, @n, @type=book, @xml:id) (multiple)
      div (@data-level=2, @n, @type=part, @xml:id) (multiple)
        head (@xml:lang=lat-Latn) (multiple)
        p (@xml:id) (multiple)
          [lb (@n) (multiple)]
          [foreign (@xml:lang=lat-Latn) (multiple)]
            hi (@rend=smallcaps)
            supplied (@reason=lost | omitted) (multiple)
      div (@data-level=2, @n, @type=part, @xml:id) (multiple)
        p (@xml:id) (multiple)
          [lb (@n) (multiple)]
          [foreign (@xml:lang=lat-Latn) (multiple)]
            supplied (@reason=lost | omitted) (multiple)
        div (@data-level=3, @n, @type=chapter, @xml:id) (multiple)
          head (@xml:lang=lat-Latn) (multiple)
          p (@xml:id) (multiple)
            supplied (@reason=lost | omitted) (multiple)
            [lb (@n) (multiple)]
            [foreign (@xml:lang=lat-Latn) (multiple)]
              hi (@rend=smallcaps) (multiple)
              supplied (@reason=lost | omitted) (multiple)
          p (@xml:id) (multiple)
            [lb (@n) (multiple)]
            [foreign (@xml:lang=lat-Latn) (multiple)]
              hi (@rend=smallcaps) (multiple)
              supplied (@reason=lost | omitted) (multiple)
      div (@data-level=2, @n, @type=part, @xml:id) (multiple)
        head (@xml:lang=lat-Latn) (multiple)
        div (@data-level=3, @n, @type=chapter, @xml:id) (multiple)
          head (@xml:lang=lat-Latn) (multiple)
          p (@xml:id) (multiple)
            supplied (@reason=lost | omitted) (multiple)
            [lb (@n) (multiple)]
            [foreign (@xml:lang=lat-Latn) (multiple)]
              supplied (@reason=lost | omitted) (multiple)
              hi (@rend=smallcaps) (multiple)
              gap (@quantity=3 | 4, @reason=lost, @unit=character) (multiple)
          p (@xml:id) (multiple)
            [lb (@n) (multiple)]
            [foreign (@xml:lang=lat-Latn) (multiple)]
              hi (@rend=smallcaps) (multiple)
              supplied (@reason=lost | omitted) (multiple)
              gap (@quantity=3, @reason=lost, @unit=character)
          head (@xml:lang=lat-Latn) (multiple)
            supplied (@reason=lost) (multiple)
          p (@xml:id)
            gap (@quantity=3, @reason=lost, @unit=character)
            supplied (@reason=lost)
            [lb (@n) (multiple)]
            [foreign (@xml:lang=lat-Latn) (multiple)]
              hi (@rend=smallcaps)
              supplied (@reason=omitted)
              gap (@quantity=5, @reason=lost, @unit=character) (multiple)
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="Gramm." xml:id="book-1" type="book" data-level="1">
				<div n="Proem." xml:id="book-1-part-1" type="part" data-level="2">
					<head xml:lang="lat-Latn">Proemium</head>
					<p xml:id="book-1-part-1-p-1">
						<lb n="1"/>
						<foreign xml:lang="lat-Latn">
							<hi rend="smallcaps">Ut</hi>ilitas iuvenum me compulit edere metrum</foreign>
						<lb n="2"/>
						<foreign xml:lang="lat-Latn">Vocibus imposita que dantur signa secunda,</foreign>
						<lb n="3"/>
						<foreign xml:lang="lat-Latn">Hec pro posse meo resignabo sermone Boemo</foreign>
						<lb n="4"/>
  ...
```
