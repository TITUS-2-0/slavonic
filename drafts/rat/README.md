# Dataset 'rat'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/slav/aruss/rat/rat.htm).

* URL: https://github.com/TITUS-2-0/slavonic/tree/main/drafts/rat/
* version: unreleased
* date: 2025-03-20

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/slavonic/tree/main/drafts/rat/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Chapter | `div@chapter` | Automatically translated into named div |
| Verse | `ab@verse` |  |

### Structural overview
```text
text (@xml:lang=orv-Cyrl)
  body
    div (@data-level=1, @n, @type=chapter, @xml:id) (multiple)
      ab (@n, @type=verse, @xml:id) (multiple)
        [foreign (@xml:lang=rus-Cyrl | und-Latn-x-general) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="chapter-1" type="chapter" data-level="1">
				<ab n="1" type="verse" xml:id="chapter-1-ab-1">
					<foreign xml:lang="rus-Cyrl">Въ началѣ Богъ сотворилъ небеса и землю.</foreign>
				</ab>
				<ab n="2" type="verse" xml:id="chapter-1-ab-2">
					<foreign xml:lang="rus-Cyrl">Но земля была не образована и пуста, и тьма надъ бездною, и Духъ Божiй носился надъ водами.</foreign>
				</ab>
				<ab n="3" type="verse" xml:id="chapter-1-ab-3">
					<foreign xml:lang="rus-Cyrl">И сказалъ Богъ: да будетъ свѣтъ; и сталъ свѣтъ.</foreign>
				</ab>
				<ab n="4" type="verse" xml:id="chapter-1-ab-4">
					<foreign xml:lang="rus-Cyrl">Богъ увидѣлъ, что свѣтъ хорошъ; и отдѣлилъ Богъ свѣтъ отъ тьмы.</foreign>
  ...
```
