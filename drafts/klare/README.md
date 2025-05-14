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
      div (@data-level=2, @n, @type=part, @xml:id, @xml:lang=lat-Latn) (multiple)
        head (multiple)
        p (@xml:id)
          hi (@rend=smallcaps)
          supplied (@reason=omitted) (multiple)
          [lb (@n) (multiple)]
        p (@xml:id)
          [lb (@n) (multiple)]
      div (@data-level=2, @n, @type=part, @xml:id) (multiple)
        p (@xml:id)
          supplied (@reason=lost) (multiple)
          [lb (@n, @xml:lang=lat-Latn) (multiple)]
        div (@data-level=3, @n, @type=chapter, @xml:id) (multiple)
          head (@xml:lang=lat-Latn) (multiple)
          p (@xml:id) (multiple)
            hi (@rend=smallcaps) (multiple)
            supplied (@reason=lost | omitted) (multiple)
            [lb (@n, @xml:lang=lat-Latn) (multiple)]
            [lb (@n) (multiple)]
            [foreign (@xml:lang=lat-Latn) (multiple)]
              supplied (@reason=lost | omitted) (multiple)
          p (@xml:id) (multiple)
            supplied (@reason=lost | omitted) (multiple)
            [lb (@n, @xml:lang=lat-Latn) (multiple)]
            [lb (@n) (multiple)]
            [foreign (@xml:lang=lat-Latn) (multiple)]
              supplied (@reason=lost | omitted) (multiple)
              hi (@rend=smallcaps) (multiple)
          p (@xml:id) (multiple)
            [lb (@n) (multiple)]
            [foreign (@xml:lang=lat-Latn) (multiple)]
              hi (@rend=smallcaps) (multiple)
            [lb (@n, @xml:lang=lat-Latn) (multiple)]
        p (@xml:id) (multiple)
          [lb (@n, @xml:lang=lat-Latn) (multiple)]
          [lb (@n)]
          [foreign (@xml:lang=lat-Latn)]
            supplied (@reason=omitted)
        div (@data-level=3, @n, @type=chapter, @xml:id, @xml:lang=lat-Latn) (multiple)
          head (multiple)
          p (@xml:id) (multiple)
            hi (@rend=smallcaps) (multiple)
            supplied (@reason=lost | omitted) (multiple)
            [lb (@n) (multiple)]
          p (@xml:id) (multiple)
            supplied (@reason=lost) (multiple)
            [lb (@n) (multiple)]
          p (@xml:id)
            hi (@rend=smallcaps)
            [lb (@n) (multiple)]
      div (@data-level=2, @n, @type=part, @xml:id)
        head (@xml:lang=lat-Latn)
        p (@xml:id)
          [lb (@n) (multiple)]
          [foreign (@xml:lang=lat-Latn) (multiple)]
            supplied (@reason=lost)
          [lb (@n, @xml:lang=lat-Latn) (multiple)]
      div (@data-level=2, @n, @type=part, @xml:id) (multiple)
        head (@xml:lang=lat-Latn) (multiple)
        div (@data-level=3, @n, @type=chapter, @xml:id) (multiple)
          head (@xml:lang=lat-Latn) (multiple)
          p (@xml:id) (multiple)
            supplied (@reason=lost | omitted) (multiple)
            [lb (@n) (multiple)]
            [foreign (@xml:lang=lat-Latn) (multiple)]
              supplied (@reason=lost | omitted) (multiple)
            [lb (@n, @xml:lang=lat-Latn) (multiple)]
          p (@xml:id) (multiple)
            hi (@rend=smallcaps) (multiple)
            [lb (@n, @xml:lang=lat-Latn) (multiple)]
            [lb (@n) (multiple)]
            [foreign (@xml:lang=lat-Latn) (multiple)]
              supplied (@reason=lost | omitted) (multiple)
              gap (@quantity=3, @reason=lost, @unit=character)
          p (@xml:id) (multiple)
            hi (@rend=smallcaps) (multiple)
            supplied (@reason=lost | omitted) (multiple)
            [lb (@n, @xml:lang=lat-Latn) (multiple)]
            [lb (@n) (multiple)]
            [foreign (@xml:lang=lat-Latn) (multiple)]
              supplied (@reason=lost | omitted) (multiple)
              gap (@quantity=3 | 4, @reason=lost, @unit=character) (multiple)
          head (@xml:lang=lat-Latn) (multiple)
            supplied (@reason=lost) (multiple)
          p (@xml:id) (multiple)
            [lb (@n, @xml:lang=lat-Latn) (multiple)]
            [lb (@n) (multiple)]
            [foreign (@xml:lang=lat-Latn) (multiple)]
              supplied (@reason=lost) (multiple)
          p (@xml:id)
            hi (@rend=smallcaps)
            gap (@quantity=3, @reason=lost, @unit=character)
            supplied (@reason=lost)
            [lb (@n, @xml:lang=lat-Latn) (multiple)]
            [lb (@n) (multiple)]
            [foreign (@xml:lang=lat-Latn) (multiple)]
              supplied (@reason=omitted)
              gap (@quantity=5, @reason=lost, @unit=character) (multiple)
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="Gramm." xml:id="book-1" type="book" data-level="1">
				<div n="Proem." xml:id="book-1-part-1" type="part" data-level="2" xml:lang="lat-Latn">
					<head>Proemium</head>
					<p xml:id="book-1-part-1-p-1">
						<lb n="1"/>
						<hi rend="smallcaps">Ut</hi>ilitas iuvenum me compulit edere metrum<lb n="2"/>Vocibus imposita que dantur signa secunda,<lb n="3"/>Hec pro posse meo resignabo sermone Boemo<lb n="4"/>Nam sine vocabulis mens inscia dicitur omnis.<lb n="5"/>Sed gratis edificat, sine Cristo quique laborat<lb n="6"/>Hic, peto, quod mecum sistens iuvet edere totum.<lb n="7"/>Ut non pervertam sensum, volo vertere que<supplied reason="omitted">n</supplied>dam,<lb n="8"/>Cui vero non placeat <supplied reason="omitted">soli</supplied>, talia vel melius eda<supplied reason="omitted">n</supplied>t. -</p>
				</div>
				<div n="A" xml:id="book-1-part-2" type="part" data-level="2">
					<p xml:id="book-1-part-2-p-2">
						<lb n="9" xml:lang="lat-Latn"/>Inprimis artes tribuam <supplied reason="lost">tibi</supplied> tres <supplied reason="lost">triviales</supplied>,<lb n="10" xml:lang="lat-Latn"/>Postea tunc tales quatuor sunt quadriviales.<lb n="11" xml:lang="lat-Latn"/>Collaterales quinque tribuam tibi, quales<lb n="12" xml:lang="lat-Latn"/>Sunt michi difficiles - prius accipe grammaticales</p>
					<div n="I" xml:id="book-1-part-2-chapter-1" type="chapter" data-level="3">
						<head xml:lang="lat-Latn">De grammatica</head>
  ...
```
