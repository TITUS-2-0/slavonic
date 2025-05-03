# Dataset 'Nawoženja'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/slav/osorb/nawozena/nawoz.htm).

* URL: https://titus2.uni-frankfurt.de/dataset/nawoz
* version: 0.1.0
* date: 2025-04-23

## Citation
```text
Digital version of Nawoženja by Jakub Bart-Ćišinski (v0.1.0). By: Rainer Gerthner, Jost Gippert, Florian Matter. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://titus2.uni-frankfurt.de/dataset/nawoz, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Strophe | `lg@chant` |  |
| Verse | `l` |  |

### Structural overview
```text
text (@xml:lang=hsb-Latn)
  body
    lg (@n, @type=chant, @xml:id) (multiple)
      head (multiple)
      l (@n, @xml:id) (multiple)
```

### Structure Example

```xml
<lg xmlns="http://www.tei-c.org/ns/1.0" n="1" type="chant" xml:id="lg-1">
				<head>Prěni spěw</head>
				<l n="1" xml:id="lg-1-l-1">Na šěsćdźesato do žnjencowej žno mi kosy z najrjeńšim</l>
				<l n="2" xml:id="lg-1-l-2">zarěča brus. Pak za hólca, za hospodarja šće tola</l>
				<l n="3" xml:id="lg-1-l-3">njepomnju krasnišich žnjow, zo by bjez komdźenja mi štož lětsa</l>
				<l n="4" xml:id="lg-1-l-4">wšo šlo zasobu. Što tola do běhanja bě mi druhdy</l>
				<l n="5" xml:id="lg-1-l-5">na syna, na wotawy! Dźěn po cyłych dnjach smy mi často</l>
				<l n="6" xml:id="lg-1-l-6">pospochi wobroćeli, roztřasowali, zo by někak</l>
				<l n="7" xml:id="lg-1-l-7">do kopjenow so nam hodźalo nož, a čwaki najtolstše</l>
				<l n="8" xml:id="lg-1-l-8">rozkopali. Wuwalaneho nimo teho pak skotej</l>
				<l n="9" xml:id="lg-1-l-9">njecha šće so, a kruwy, kiž ze spěšnišim tola hewak</l>
				<l n="10" xml:id="lg-1-l-10">padaju do syna, na natykane nam ze synom rěble</l>
  ...
```
