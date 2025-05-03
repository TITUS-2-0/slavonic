# Dataset 'The Rezian Catechism I'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/slav/asloven/rezkat/rezka.htm).

* URL: https://github.com/TITUS-2-0/slavonic/tree/main/drafts/rezka/
* version: unreleased
* date: 2025-03-07

## Citation
```text
Digital version of The Rezian Catechism I (draft version). By: Jost Gippert, Florian Matter, Han Steenwijk. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/slavonic/tree/main/drafts/rezka/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Section | `div@section` | Automatically translated into named div |
| Sentence | `s` |  |
| Subdivision | `milestone@subdivision` |  |
| Page | `pb` |  |

### Structural overview
```text
text (@xml:lang=slv-Latn-x-oldslv)
  front (@xml:id)
    p (@xml:id)
      s (@n, @xml:id)
  body
    p (@xml:id)
      s (@n, @xml:id)
        [note (@xml:id)]
          [foreign (@xml:lang=deu-Latn | slv-Latn-x-rezgni) (multiple)]
    div (@data-level=1, @n, @type=section, @xml:id) (multiple)
      p (@xml:id) (multiple)
        s (@n, @xml:id) (multiple)
          [milestone (@n, @unit=subdivision, @xml:id) (multiple)]
          [note (@xml:id) (multiple)]
            [foreign (@xml:lang=deu-Latn | slv-Latn-x-rezgni | slv-Latn-x-rezsg) (multiple)]
          [foreign (@xml:lang=deu-Latn | lat-Latn | slv-Latn-x-rez | slv-Latn-x-rezgni) (multiple)]
            [note (@xml:id) (multiple)]
              [lb (@n) (multiple)]
              [foreign (@xml:lang=deu-Latn | slv-Latn-x-rezgni | slv-Latn-x-rezsg) (multiple)]
                [lb (@n) (multiple)]
                [foreign (@xml:lang=deu-Latn)]
            [lb (@n) (multiple)]
            [foreign (@xml:lang=slv-Latn-x-rez) (multiple)]
              [note (@xml:id) (multiple)]
                [lb (@n) (multiple)]
        [milestone (@n, @unit=subdivision, @xml:id)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="section-1" type="section" data-level="1">
				<p xml:id="section-1-p-3">
					<s n="3" xml:id="section-1-p-3-s-3">Tè dua Misteriha principal.<milestone unit="subdivision" n="1" xml:id="section-1-p-3-s-3-milestone-1"/>
					</s>
					<s n="4" xml:id="section-1-p-3-s-4">Tè parvi misterih iè dan sami Buh, dishtint tuv treh Persunah, chà ni sè clizzajo, Oggià, Sin, anù Sveti Duh, s nò samo bisido Santissima Trinitat.<milestone unit="subdivision" n="2" xml:id="section-1-p-3-s-4-milestone-2"/>
					</s>
					<s n="5" xml:id="section-1-p-3-s-5">Tè sehond misterih, dà ta sehond persuna, chà to jè Sin, an jè se sdelal zlovech tuv svotè od Marie Vergine, an jè patel anù umar sa nas<note xml:id="section-1-p-3-s-5-note-2">
							<foreign xml:lang="deu-Latn">S. 182:</foreign>
							<foreign xml:lang="slv-Latn-x-rezgni">zá nas, rîšnike.</foreign>
						</note> tanà Crishu, an sè clizze Giesù Crisht, nash Redentor, ver Buh, anù ver zlovech.</s>
				</p>
			</div>
```
