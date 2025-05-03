# Dataset 'The Old Czech Alexandreis'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/slav/acech/alex/alex.htm).

* URL: https://github.com/TITUS-2-0/slavonic/tree/main/drafts/alex/
* version: unreleased
* date: 2025-03-25

## Citation
```text
Digital version of The Old Czech Alexandreis (draft version). By: Jost Gippert, Florian Matter, Petr Vavroušek. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/slavonic/tree/main/drafts/alex/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Fragment | `div@fragment` | Automatically translated into named div |
| Verse | `l` |  |
| Manuscript page | `pb@manuscript` |  |

### Structural overview
```text
text (@xml:lang=ces-Latn-x-old-czech)
  body
    div (@data-level=1, @n, @type=fragment, @xml:id) (multiple)
      head (multiple)
        [foreign (@xml:lang=ces-Latn) (multiple)]
      lg (@n, @type=stanza, @xml:id) (multiple)
        l (@n, @xml:id) (multiple)
          [pb (@n, @type=manuscript) (multiple)]
        l (@n, @xml:id) (multiple)
          gap (@reason=lost, @unit=characters) (multiple)
      lg (@n, @type=stanza, @xml:id) (multiple)
        l (@n, @xml:id) (multiple)
          [pb (@n, @type=manuscript) (multiple)]
        gap (@reason=lost, @unit=line) (multiple)
        l (@n, @xml:id) (multiple)
          gap (@reason=lost, @unit=characters) (multiple)
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="AlxV" xml:id="fragment-1" type="fragment" data-level="1">
				<head>
					<foreign xml:lang="ces-Latn">ZLOMEK SVATOVÍTSKÝ -</foreign>
				</head>
				<lg type="stanza" n="1" xml:id="fragment-1-lg-1">
					<l n="1" xml:id="fragment-1-lg-1-l-1">Jenž ze jmene byl věhlasný,</l>
					<l n="2" xml:id="fragment-1-lg-1-l-2">jehož rozum byl tak jasný,</l>
					<l n="3" xml:id="fragment-1-lg-1-l-3">že jmu bylo všecko známo</l>
					<l n="4" xml:id="fragment-1-lg-1-l-4">vzemi, vmoři, vhvězdách tamo,</l>
					<l n="5" xml:id="fragment-1-lg-1-l-5">ten však čtveru věc vyčítá,</l>
					<l n="6" xml:id="fragment-1-lg-1-l-6">jež přěd jeho smyslem skryta:</l>
					<l n="7" xml:id="fragment-1-lg-1-l-7">"Kak mám", pravě, "sirdce radné,</l>
  ...
```
