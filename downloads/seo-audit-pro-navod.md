# SEO Audit Pro — přesný návod a checklist

Tento návod je pracovní podklad pro malý firemní web. Pomůže připravit audit, popsat opravy a zkontrolovat jejich nasazení. **Neslibuje pozice ani konkrétní návštěvnost.** Google vytváří výsledky automaticky a dopad změn je potřeba vyhodnocovat v čase.[1]

## Co si připravit před auditem

Sepište hlavní cíl webu, jednu až tři služby nebo kategorie, které mají přivádět poptávky, a seznam URL, které jsou pro tento cíl důležité. U malého webu obvykle stačí homepage, hlavní služby, kontakt a vybrané referenční nebo produktové stránky.

Zapište si také, kdo může upravovat obsah, kdo spravuje hosting a zda máte přístup do Search Console, analytiky nebo redakčního systému. Audit bez těchto informací stále odhalí veřejně viditelné problémy, ale neověří vše, co se děje po přihlášení.

## 1. Záměr každé důležité stránky

U každé URL vyplňte tuto větu:

> Tato stránka má pomoci **[komu]** rozhodnout se pro **[konkrétní službu / produkt]** a dovést ho k **[dalšímu kroku]**.

Pokud větu nejde napsat jednoduše, stránka pravděpodobně spojuje více záměrů. Nejprve upravte obsahovou strukturu. Teprve pak řešte title nebo klíčová slova.

## 2. Title, meta description a H1

Pro každou kontrolovanou URL si připravte tři odlišné prvky:

- **Title:** stručný, jedinečný titul stránky. Má přesně popsat, co uživatel na stránce najde.
- **Meta description:** věcný souhrn konkrétní stránky. Neopakujte stejný popis na všech URL a nepište jen výčet výrazů.[2]
- **H1:** hlavní nadpis viditelný návštěvníkovi. Musí odpovídat skutečnému obsahu a záměru URL.

Pracovní šablona:

```text
Title: [služba nebo produkt] pro [cílovou situaci] | [značka]
Meta description: [co stránka konkrétně řeší] + [důkaz / rozsah] + [smysluplný další krok].
H1: [jasný výsledek nebo nabídka pro návštěvníka].
```

### Reálná ukázka ROSTIVO

Na veřejné produktové stránce Stavby Pro je použit tento konkrétní zápis:

```html
<title>Stavby Pro — šablona pro stavby a rekonstrukce | ROSTIVO</title>
<meta name="description" content="Stavby Pro je hotová webová šablona pro stavební firmy a rekonstrukce s variantami odborného nasazení od ROSTIVO." />
<link rel="canonical" href="https://rostivo.studio/digitalni-produkty/stavby-pro/" />
```

Je to ukázka popisu konkrétní nabídky. Není to tvrzení o pozici, návštěvnosti ani výsledku klienta. Živý veřejný výstup je k dispozici na [GitHub Pages ROSTIVO](https://rostivocz-dotcom.github.io/digitalni-produkty/stavby-pro/).

## 3. Indexace, canonical, sitemap a robots

U každé důležité URL ověřte:

1. Otevírá se správná stránka a není to pouze přesměrování na jiný obsah?
2. Je ve zdrojovém HTML uvedená správná canonical URL?
3. Je preferovaná URL uvedená v `sitemap.xml`?
4. Neblokuje ji `robots.txt`, meta robots nebo přístupové omezení?
5. Obsahuje stránka skutečný H1 a text i bez čekání na JavaScript?

Sitemap pomáhá vyhledávači objevit URL, ale sama o sobě nezaručuje indexaci ani pozici. Důležitější je hodnotný, přístupný obsah a srozumitelná struktura webu.[1]

## 4. Obsah a interní odkazy

U každé klíčové stránky zkontrolujte:

- Odpovídá první odstavec na základní otázku zákazníka?
- Jsou služby, postup, podklady a další krok vysvětlené bez marketingové vaty?
- Vedou z příbuzných stránek přirozené odkazy na tuto URL?
- Existuje vedle odkazu krátké vysvětlení, proč je další stránka relevantní?
- Jsou fotografie popsané alternativním textem podle skutečného obsahu obrázku?

Nepřidávejte text jen proto, aby byl delší. Google doporučuje obsah, který je čitelný, vlastní, aktuální a užitečný pro člověka.[1]

## 5. Strukturovaná data

Strukturovaná data mají doplňovat to, co návštěvník na stránce opravdu vidí. Nezakládejte prázdné stránky jen kvůli JSON-LD a nevkládejte údaje, které nejsou viditelné nebo nejsou přesné.[3]

Pracovní kontrola:

```text
[ ] Typ schématu odpovídá stránce (např. Product, Service, Article).
[ ] Název, popis, cena a dostupnost odpovídají viditelnému obsahu.
[ ] Všechny povinné údaje jsou uvedené přesně.
[ ] Výstup je ověřený v Rich Results Testu, pokud je daný typ podporovaný.
```

## 6. Kontrola po nasazení

Po úpravách nepovažujte práci za hotovou, dokud neověříte skutečně servírovanou stránku:

```bash
curl -I https://vas-web.cz/vase-stranka/
curl -L https://vas-web.cz/vase-stranka/ | grep -E "<title>|description|canonical"
```

Zkontrolujte stav odpovědi, title, description, canonical, hlavní nadpis, interní odkazy a případná strukturovaná data. U zásadních změn přidejte URL do Search Console a sledujte její stav. Změny se mohou promítnout během hodin až měsíců; vyhodnocujte je až na dostatečně dlouhém období.[1]

## Co zahrnují balíčky SEO Audit Pro

### SEO Audit Start — 8 900 Kč

- Audit až 10 klíčových URL.
- Indexace, title, meta, nadpisy, canonical, sitemap a robots.
- Kontrola obrázků, odkazů a veřejně viditelných technických chyb.
- Prioritizovaný checklist a 45min online vysvětlení.

### SEO Audit + implementace — 14 900 Kč

- Vše ze SEO Audit Start.
- Domluvené úpravy title, meta, nadpisů a interních odkazů až na 15 klíčových URL.
- Jeden návrh obsahové struktury pro důležitou službu nebo kategorii.
- Kontrola po nasazení a předání změn.

### SEO Péče — 4 900 Kč / měsíc

- Měsíční kontrola indexace, chyb a priorit.
- Kontrola jedné nové nebo upravené stránky před publikací.
- Krátký report s doporučenými dalšími kroky.

Cena je výchozí cena pro malý firemní web. Daňový režim, termín, technický rozsah a dostupné přístupy se potvrzují v konkrétní nabídce před zahájením práce. Balíčky nezahrnují vývoj nad uvedený rozsah, kompletní copywriting, placené SEO nástroje ani linkbuilding, pokud nejsou výslovně domluveny.

## Zdroje

[1]: https://developers.google.com/search/docs/fundamentals/seo-starter-guide "Google Search Central — SEO Starter Guide"
[2]: https://developers.google.com/search/docs/appearance/snippet "Google Search Central — Control your snippets in search results"
[3]: https://developers.google.com/search/docs/appearance/structured-data/intro-structured-data "Google Search Central — Introduction to structured data markup"
