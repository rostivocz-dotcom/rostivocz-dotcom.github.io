# SEO Viditelnost Pro — ukázková kapitola

Toto je **ukázka digitálního produktu SEO Viditelnost Pro**. Plný balíček za **2 490 Kč** obsahuje návod od A do Z, pracovní šablony, checklisty, reálnou ukázku a 30denní postup. Ukázka níže vysvětluje, jak pracovat s jednou důležitou URL.

> SEO není slib první pozice. Cílem je vytvořit srozumitelný, přístupný a technicky čitelný základ, který vyhledávače i zákazníci dokážou pochopit.[1]

## 1. Určete jeden účel URL

U každé důležité stránky doplňte větu:

> Tato stránka pomáhá **[konkrétnímu typu zákazníka]** rozhodnout se pro **[službu nebo produkt]** a dovést ho k **[dalšímu kroku]**.

Pokud na jednu URL patří několik různých služeb nebo záměrů, nerozšiřujte bezmyšlenkovitě text. Nejprve zvažte samostatné stránky a smysluplné interní odkazy mezi nimi.

## 2. Připravte title, meta description a H1

Použijte tři rozdílné, ale obsahově související prvky:

```text
Title: [služba nebo produkt] pro [cílovou situaci] | [značka]
Meta description: [co stránka konkrétně řeší] + [důkaz nebo rozsah] + [další krok].
H1: [jasný výsledek nebo nabídka pro návštěvníka].
```

Meta description nemá být výčet výrazů. Má stručně vysvětlit konkrétní obsah URL. Google může pro výsledky vyhledávání použít obsah stránky nebo description podle toho, co lépe odpovídá dotazu.[2]

## 3. Reálná ukázka ROSTIVO

Na veřejné produktové stránce Stavby Pro je použit tento zápis:

```html
<title>Stavby Pro — šablona pro stavby a rekonstrukce | ROSTIVO</title>
<meta name="description" content="Stavby Pro je hotová webová šablona pro stavební firmy a rekonstrukce s variantami odborného nasazení od ROSTIVO." />
<link rel="canonical" href="https://rostivo.studio/digitalni-produkty/stavby-pro/" />
```

Ukázka popisuje konkrétní nabídku. **Není to případová studie ani tvrzení o pozicích, návštěvnosti nebo výsledku klienta.** Veřejný výstup si můžete otevřít na [GitHub Pages ROSTIVO](https://rostivocz-dotcom.github.io/digitalni-produkty/stavby-pro/).

## 4. Kontrola po opravě

Po nasazení ověřte, zda je veřejná verze opravdu aktualizovaná:

```bash
curl -I https://vas-web.cz/vase-stranka/
curl -L https://vas-web.cz/vase-stranka/ | grep -E "<title>|description|canonical"
```

Zkontrolujte stav odpovědi, title, description, canonical a hlavní nadpis. U větších změn pokračujte kontrolou v Search Console. Sitemapa pomáhá URL objevit, ale sama o sobě nezaručuje indexaci ani pozici.[1]

## Co je v plném digitálním balíčku

- krokový návod od A do Z;
- pracovní šablony pro mapu URL, title, meta description a priority oprav;
- checklist pro indexaci, canonical, sitemap, robots, obrázky, interní odkazy a strukturovaná data;
- návod pro kontrolu před a po publikaci;
- 30denní plán samostatné práce;
- reálná ukázka ROSTIVO.

Pro web, kde chcete provést audit a základní vylepšení odborně, je k dispozici **SEO audit + vylepšení od 9 600 Kč**. Výchozí rozsah zahrnuje audit do 10 klíčových URL, prioritní plán oprav, domluvené základní on-page změny a online předání. Rozsah se vždy potvrdí před objednávkou.

## Zdroje

[1]: https://developers.google.com/search/docs/fundamentals/seo-starter-guide "Google Search Central — SEO Starter Guide"
[2]: https://developers.google.com/search/docs/appearance/snippet "Google Search Central — Control your snippets in search results"
