# Dataset 'Junosti Čestnoe Zercalo'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/slav/aruss/sercalo/serca.htm).

* URL: https://github.com/TITUS-2-0/slavonic/tree/main/drafts/serca/
* version: unreleased
* date: 2025-03-20

## Citation
```text
Digital version of Junosti Čestnoe Zercalo (draft version). By: Vladimir Alekseev, Jost Gippert, Florian Matter. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/slavonic/tree/main/drafts/serca/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Chapter | `div@chapter` | Automatically translated into named div |
| Paragraph | `p` |  |
| Sentence | `s` |  |
| Page | `pb` |  |
| Line | `lb` |  |

### Structural overview
```text
text (@xml:lang=orv-Cyrl)
  body
    div (@data-level=1, @n, @type=chapter, @xml:id)
      p (@n, @xml:id) (multiple)
        s (@n, @xml:id) (multiple)
          [lb (@n) (multiple)]
          [pb (@n) (multiple)]
          [foreign (@xml:lang=rus-Cyrl) (multiple)]
            [lb (@n) (multiple)]
            [pb (@n) (multiple)]
        [lb (@n) (multiple)]
        [pb (@n) (multiple)]
      [pb (@n)]
      [lb (@n)]
    div (@data-level=1, @n, @type=chapter, @xml:id) (multiple)
      head (@xml:lang=rus-Cyrl) (multiple)
      p (@n, @xml:id) (multiple)
        s (@n, @xml:id) (multiple)
          [lb (@n) (multiple)]
          [pb (@n) (multiple)]
          [foreign (@xml:lang=rus-Cyrl) (multiple)]
            [lb (@n) (multiple)]
            [pb (@n) (multiple)]
        [lb (@n) (multiple)]
        [pb (@n) (multiple)]
      [lb (@n) (multiple)]
      [pb (@n) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="chapter-1" type="chapter" data-level="1">
				<pb n="1"/>
				<lb n="7"/>
				<p n="1." xml:id="chapter-1-p-1">
					<s n="1" xml:id="chapter-1-p-1-s-1">Въ первыхъ наïпаче всего должни дѣти отца и матерь въ велïкои чести<lb n="10"/>содержать.</s>
					<s n="2" xml:id="chapter-1-p-1-s-2">И когда отъ родïтелеи что имъ прïказано бываетъ, всегда шляпу въ рукахъ держать, а пред нïми не вздѣвать, и возлѣ ихъ не садïтïся, и прежде<lb n="15"/>оныхъ не засѣдать, при нïхъ во окно всѣмъ тѣломъ не выглядовать,<lb n="17"/>но все потаеннымъ образомъ<pb n="2"/>
						<lb n="1"/>съ велïкïмъ почтенïемъ, не съ нïми врядъ, но немного уступя позади оныхъ къ сторонѣ стоять, подобно яко пажъ нѣкоторыи или слуга.<lb n="5"/>
					</s>
					<s n="3" xml:id="chapter-1-p-1-s-3">Въ домѣ нïчего своïмъ имянемъ не повелѣвать, но имянемъ отца или матере, от челядïнцѣвъ просïтелнымъ образомъ требовать, развѣ что у кого особлïвыя слуги,<lb n="10"/>которыя самому ему подвержены бываютъ.</s>
					<s n="4" xml:id="chapter-1-p-1-s-4">для того, что обычаïно служïтели и челядïнцы не двумъ господамъ и госпожамъ, но токмо одному господïну охотно служатъ.<lb n="15"/>
					</s>
					<s n="5" xml:id="chapter-1-p-1-s-5">
  ...
```
