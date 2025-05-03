# Dataset 'supra'

![Static Badge](https://img.shields.io/badge/TEI_validation-failing-red)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/slav/aksl/suprasl/supra.htm).

* URL: https://github.com/TITUS-2-0/slavonic/tree/main/drafts/supra/
* version: unreleased
* date: 2025-04-10

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/slavonic/tree/main/drafts/supra/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Chapter | `div@chapter` | Automatically translated into named div |
| Page of ed. | `pb@edition` |  |
| Ms. page | `pb@manuscript` |  |
| Line | `lb@edition` |  |

### Structural overview
```text
text (@xml:lang=chu-Glag)
  body
    div (@data-level=1, @n, @type=part, @xml:id) (multiple)
      head (@xml:lang=lat-Latn) (multiple)
      div (@data-level=2, @n, @type=chapter, @xml:id) (multiple)
        head (@xml:lang=lat-Latn) (multiple)
        [pb (@n, @type=edition | manuscript) (multiple)]
        [lb (@n, @type=edition) (multiple)]
      div (@data-level=2, @n, @type=chapter, @xml:id) (multiple)
        [foreign (@xml:lang=und-Latn-x-general) (multiple)]
        [pb (@n, @type=edition | manuscript) (multiple)]
        [lb (@n, @type=edition) (multiple)]
      [pb (@n, @type=edition | manuscript) (multiple)]
      [lb (@n, @type=edition) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="part-1" type="part" data-level="1">
				<head xml:lang="lat-Latn">Manus prima</head>
				<div n="1" xml:id="part-1-chapter-1" type="chapter" data-level="2">
					<head xml:lang="lat-Latn">Cap. 1</head>
					<pb type="manuscript" n="1a"/>
					<pb type="edition" n="1"/>
					<lb type="edition" n="1"/>мы῾ихъ бо ῾отъ бога ῾эсвѣ · твоэи бо<lb type="edition" n="2"/>доуши погыбѣл᾽ь прѣ῾одолѣ дожи<lb type="edition" n="3"/>᾽и до съмр᾽ьти · не добрѣ мѫдрова-<lb type="edition" n="4"/>ти на цѣломѫдрованиэ къ богоу ·<lb type="edition" n="5"/>много бо бѣсовани῾э ῾эже отъ тебе то-<lb type="edition" n="6"/>мьэниэ въвръже тѧ въ хоулѫ · ῾аг᾽ге̑-<lb type="edition" n="7"/>ла бо ῾эгоже посъла г҃ь ї҃с х҃с ῾и б҃ъ · ӡагра-<lb type="edition" n="8"/>ди оу̑ста плѣжѫштиїхъ · ῾эгоже ты<lb type="edition" n="9"/>сво῾имъ прѣӡор᾽ьствомъ прѣложи въ<lb type="edition" n="10"/>аполона · ῾и раӡгнѣвавъ сѧ ῾аурилия-<lb type="edition" n="11"/>нъ повелѣ съвалъмы оловѣны битi<lb type="edition" n="12"/>я по челюст᾽ьма · глагољѧ ῾эмоу не ῾ѫро-<lb type="edition" n="13"/>д᾽ьно ῾и прѣӡор᾽ьно ῾отъвѣштава᾽и ·<lb type="edition" n="14"/>вѣды ῾яко прѣдъ цѣсаремь сто῾иши ·<lb type="edition" n="15"/>и ῾отъведъ паула свѣње сѫдиїшта прi-<lb type="edition" n="16"/>ӡъвавъ ῾иоу̑ли῾яниѭ̑ рече къ ње᾽и ·<lb type="edition" n="17"/>владычице мо῾эѧ д҃шѧ ῾иоу̑лияниэ ·<lb type="edition" n="18"/>оу̑мољена быв᾽ши ῾отъ мене · не прѣљь-<lb type="edition" n="19"/>штаи сѧ боуэстиѭ̑ пав᾽ьла брата сво-<lb type="edition" n="20"/>῾эго · виждѫ бо тѧ дѣвицѫ мѫдрѫ сѫ-<lb type="edition" n="21"/>штѫ · ῾и м᾽ногѫ прѣмѫдрость имѫштѫ ·<lb type="edition" n="22"/>да оу̑тѣшивъши сѧ послоуша᾽и мене ·<lb type="edition" n="23"/>и бѫдеши владычица мо῾эи д҃ши · и о-<lb type="edition" n="24"/>браӡы ӡлаты поставьѭ̑ ти по в᾽ьсѧ<lb type="edition" n="25"/>грады в᾽ьсеѧ в᾽ьсељены᾽ѧ · ῾отъвѣшта-<lb type="edition" n="26"/>въши же ῾иоу̑лияни рече · не ῾отъвръ-<lb type="edition" n="27"/>гѫ сѧ аурили῾яне томителю ῾и непрѣ-<lb type="edition" n="28"/>подобьне · не прѣл᾽ьстиши рабы бо-<lb type="edition" n="29"/>га вышьняаго · не примышля῾и ми<lb type="edition" n="30"/>съмрьти вѣч᾽ьныѧ лишити мѧ хотѧ<pb type="manuscript" n="1b"/>
					<pb type="edition" n="2"/>
					<lb type="edition" n="1"/>славы х҃совы · и цѣсарьства небесънаа-<lb type="edition" n="2"/>го· ῾эгоже ты штоуждъ ῾эси · ῾и ῾отъвед<lb type="edition" n="3"/>ѭ̑ повелѣ прити паулоу · ῾и рече ῾эмоу<lb type="edition" n="4"/>павьле · ῾иоу̑лияни сестра твоя ῾обѣшта<lb type="edition" n="5"/>сѧ пожр᾽ьти богомъ · ῾и быти ῾э᾽и женѣ<lb type="edition" n="6"/>ми и госпожди цѣсар᾽ьствоу мо῾эмоу ·<lb type="edition" n="7"/>въсхошти оу̑бо ῾и ты тожде мѫдроватi<lb type="edition" n="8"/>῾и пристѫпивъ пож᾽ьри богомъ · паулъ<lb type="edition" n="9"/>рече · прав᾽ь сълъга · ничесоже штоу-<lb type="edition" n="10"/>жда сътвори наоу̑чения ῾от᾽ьца тво῾эго<lb type="edition" n="11"/>диявола · не можеши бо никогоже ῾отъ-<lb type="edition" n="12"/>тръгнѫти · раӡвѣ лъжеѭ̑ · насъ же не ῾и-<lb type="edition" n="13"/>маши въсхытити · ῾аште ῾и цѣсар᾽ьство҃<lb type="edition" n="14"/>намъ ῾обѣштава῾эши · ῾эгоже ты лихъ<lb type="edition" n="15"/>эси · ῾аурили῾янъ рече · доколѣ досажда-<lb type="edition" n="16"/>῾эши не срам᾽ь῾я῾ѧ сѧ ῾ѫроде ῾и беӡоум᾽ьлю ·<lb type="edition" n="17"/>тако ми богы ῾аӡъ ва имамъ мѫчити ·<lb type="edition" n="18"/>да ник᾽тоже въӡможетъ помошти ва-<lb type="edition" n="19"/>ма · ῾и повелѣ принести ῾огњь · ῾и полицѧ<lb type="edition" n="20"/>желѣӡны · ῾и въложити ѧ въ огњь · и па-<lb type="edition" n="21"/>улоу съвѧӡати рѫцѣ ῾и ноӡѣ · ῾и колъ же-<lb type="edition" n="22"/>лѣӡнъ въврѣти междоу рѫкама ῾и но-<lb type="edition" n="23"/>гама · ῾и вънъӡнѫти в᾽ь ӡемьѭ̑ · ῾и д᾽вѣ-<lb type="edition" n="24"/>ма митѣ палицама      нама битi ᾽и ·<lb type="edition" n="25"/>и ї҃оу̑ли῾яниѭ̑ повелѣ поставити на блѫ-<lb type="edition" n="26"/>дилишти · рек᾽ше на цѧто῾им᾽ьствѣ ·<lb type="edition" n="27"/>и м᾽ноӡи ῾отъ сто῾ѧштааго тоу народа ·<lb type="edition" n="28"/>бѣ῾ахѫ текѫште · ῾и р᾽ьвъноуѭ̑ште кѹ-<lb type="edition" n="29"/>п᾽ьно · к᾽то пр᾽ьво᾽э вьнидет᾽ь къ ње᾽и ·<lb type="edition" n="30"/>бѣ῾ахѫ бо ῾яко коњи ръжѫште ῾о добротѣ<pb type="manuscript" n="2a"/>
					<pb type="edition" n="3"/>
					<lb type="edition" n="1"/>эѧ · став᾽ши же ῾эи на мѣстѣ на њем᾽же<lb type="edition" n="2"/>повелѣ ῾аурилиянъ · ῾и абиэ ᾽аг᾽ге̑лъ г҃нь<lb type="edition" n="3"/>прѣдъста прѣдъ њеѭ̑ · глагољѧ · не оу̑-<lb type="edition" n="4"/>бо᾽и сѧ ῾иоули῾яни· г҃ь бо ї҃с х҃с ῾эмоуже ты<lb type="edition" n="5"/>слоужиши посъла мѧ покрыти тѧ ·<lb type="edition" n="6"/>и покаӡати свѧтоэ ῾имѧ эго в᾽ьсѣмъ<lb type="edition" n="7"/>бо῾ѧштиїмъ сѧ ῾эго · и ῾яко отъ желани-<lb type="edition" n="8"/>я къ ῾ию̑ли᾽яниї теча῾ахѫ народи в᾽ьси ·<lb type="edition" n="9"/>῾аг᾽ге̑лъ же ῾отътрѧсъ прахъ ῾яко ῾отъ но-<lb type="edition" n="10"/>гъ ᾽ихъ · ῾ослѣпи ѧ ῾и не вѣдѣ῾ахѫ камо<lb type="edition" n="11"/>῾идѫтъ · ῾и не можа῾ахѫ приближити сѧ<lb type="edition" n="12"/>῾эи · ῾и в᾽ьпи῾яхѫ в᾽ьси народи коуп᾽но<lb type="edition" n="13"/>глагољѫште · великъ богъ пауљь ῾и їоу̑-<lb type="edition" n="14"/>лиянинъ · иже в᾽ьс᾽ьде съпасъ и покро-<lb type="edition" n="15"/>витељь боѧштиїхъ сѧ ῾эго · ῾и прѣбыва-<lb type="edition" n="16"/>хѫ ῾эште слѣпи · пришьдъше же покла-<lb type="edition" n="17"/>ня᾽ахѫ сѧ ῾э᾽и · в᾽ьпиѭ̑ште ῾и глагољѫште ·<lb type="edition" n="18"/>῾иоу̑ли῾яниэ рабо б҃а выш᾽ьняго · съгрѣ-<lb type="edition" n="19"/>шихомъ прѣдъ тобоѭ̑ ῾ѫродъскы · нъ<lb type="edition" n="20"/>простивъши ны ῾яко блага бога слоужи-<lb type="edition" n="21"/>тељьница · помоли сѧ х҃соу да подастъ<lb type="edition" n="22"/>намъ видѣни῾я · С҃та῾а же ῾иоу̑ли῾яни<lb type="edition" n="23"/>милоср᾽ьдовавъши в᾽ьӡѧ воды мало ·<lb type="edition" n="24"/>и въӡвед᾽ши ῾очи свои на небо · помоли<lb type="edition" n="25"/>сѧ богоу глагољѫшти · г҃и ї҃с х҃се с҃псе в᾽ь-<lb type="edition" n="26"/>сѣхъ ч҃лкъ · оу̑слыши мене ῾и покажи ·<lb type="edition" n="27"/>чоудеса сво῾я ῾яже твориши с҃номъ чло-<lb type="edition" n="28"/>вѣчьскомъ · ῾и даръствоу᾽и ᾽имъ видѣ-<lb type="edition" n="29"/>ни᾽э · да прославѧтъ с҃тоэ ῾и прѣхвал᾽ь-<lb type="edition" n="30"/>ноэ ῾имѧ тво᾽э · ῾и тако покропи в᾽ьсь народ᾽ ·<pb type="manuscript" n="2b"/>
					<pb type="edition" n="4"/>
  ...
```
