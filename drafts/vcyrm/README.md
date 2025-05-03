# Dataset 'vcyrm'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcc/slav/aksl/vcyrmeth/vcyrm.htm).

* URL: https://github.com/TITUS-2-0/slavonic/tree/main/drafts/vcyrm/
* version: unreleased
* date: 2025-04-09

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/slavonic/tree/main/drafts/vcyrm/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Chapter | `div@chapter` | Automatically translated into named div |
| Paragraph | `p` |  |
| Line | `lb` |  |

### Structural overview
```text
text (@xml:lang=chu-Glag)
  body
    p (@xml:id)
      [lb (@n) (multiple)]
    div (@data-level=1, @n, @type=chapter, @xml:id) (multiple)
      p (@n, @xml:id) (multiple)
        [lb (@n) (multiple)]
        [foreign (@xml:lang=lat-Latn)]
      [pb (@n) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="chapter-1" type="chapter" data-level="1">
				<pb n="1"/>
				<p n="1" xml:id="chapter-1-p-2">
					<lb n="1"/>Богъ милостивь и щедрь· ѡжидаэ покааніе чловѣчьско· да<lb n="2"/>быше въси съпасены были и въ раӡѹмь истин/ныи пришли· не<lb n="3"/>хощет/ бо съмр/ти грѣшникѹ· нъ покаянію и животѹ· аще и<lb n="4"/>наипаче приложить на ӡлобѹ· нъ не ѡставляэть чловѣча<lb n="5"/>рода ѡтпасти ѡслаблэніемь и вь сьблаӡнь неприяӡнинѹ<lb n="6"/>пріити и погыбнѹти· нъ на каяжда лѣта и врѣмена не<lb n="7"/>прѣстаэть благодать творе намь мнѡго· яко испрьва<lb n="8"/>даже и до ныня· патриарьхи же пръвѣе и ѡтьци и по тѣхь<lb n="9"/>пророкы· а по сихь апостоли и моученикы· праведными моужи<lb n="10"/>и оучители иӡбираэи ѡть многомльвнаго житіа сего·</p>
				<pb n="2"/>
				<p n="2" xml:id="chapter-1-p-3">
					<lb n="1"/>ӡнаеть бо господь своэ· иже эго соуть· якоже рече· ѡв/це<lb n="2"/>моэ гласа моэго слышеть и аӡь ӡнаю э и именемь въӡываю<lb n="3"/>э и по мнѣ ходеть и даю имь животь вѣч/ныи·</p>
				<pb n="3"/>
				<p n="3" xml:id="chapter-1-p-4">
					<lb n="1"/>эже сътворіи и въ нашь родь· въӡдвигь намь оучителя<lb n="2"/>сице· иже просвѣти еӡыкь нашь· слабостію омрач/ше оумь<lb n="3"/>свои· паче льстию діаволэю· не хотѣвше въ свѣтѣ<lb n="4"/>божіихь ӡаповѣдехь ходити·</p>
				<pb n="4"/>
				<p n="4" xml:id="chapter-1-p-5">
  ...
```
