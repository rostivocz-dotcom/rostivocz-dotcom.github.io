# Core Web Vitals Pro — ukázková kapitola

Toto je **ukázka digitálního produktu Core Web Vitals Pro**. Plný balíček za **2 490 Kč** obsahuje postup od výchozího měření přes opravy LCP, INP a CLS až po kontrolu v reálném provozu, pracovní šablony a 30denní plán.

> Core Web Vitals popisují skutečnou uživatelskou zkušenost s načítáním, odezvou a vizuální stabilitou. Nejsou samostatnou garancí pozic ve vyhledávání.[1]

## 1. Nejdřív oddělte terénní a laboratorní data

Začněte na [PageSpeed Insights](https://pagespeed.web.dev/). Terénní data vycházejí z anonymizovaných návštěv za přibližně 28 dnů. Laboratorní test je řízené načtení pro diagnostiku; je užitečný pro hledání příčiny, ale nemůže nahradit reálné interakce návštěvníků.[2]

Do pracovního listu si zapište:

```text
URL nebo skupina URL:
Zařízení: mobil / desktop
Terénní LCP / INP / CLS:
Laboratorní LCP / TBT / CLS:
Největší prvek nad přehybem:
Nejdelší úloha JavaScriptu:
Prvek, který posunul rozvržení:
```

## 2. Co znamená dobrý výsledek

Google doporučuje pro dobrou uživatelskou zkušenost:

- **LCP do 2,5 s** — rychlost zobrazení hlavního obsahu;
- **INP do 200 ms** — odezva na interakci;
- **CLS do 0,1** — stabilita rozvržení.

Pro splnění prahů má cíli odpovídat 75. percentil návštěv pro všechny tři metriky.[1]

## 3. Ukázka opravy CLS: rezervujte obrazový prostor

Pokud prohlížeč nezná rozměr média před jeho stažením, může pozdější vykreslení vytlačit text a tlačítka. Začněte kontrolou skutečně publikovaného HTML:

```html
<picture>
  <source srcset="/media/hero.webp" type="image/webp" />
  <img src="/media/hero.jpg" width="2200" height="1467"
       alt="Popis hlavního obrázku" fetchpriority="high" decoding="async" />
</picture>
```

Atributy `width` a `height` dávají prohlížeči poměr stran, ze kterého může rezervovat místo. Neznamená to, že každý obrázek má být priorita pro LCP; prioritní načítání patří jen skutečně hlavnímu, viditelnému obsahu.

## 4. Ověřte změnu správným způsobem

1. Ověřte produkční URL v DevTools nebo Lighthouse a zaznamenejte změnu ve stejné testovací konfiguraci.
2. Otevřete stránku na mobilu a zkontrolujte, zda obsah při načítání neskáče.
3. Sledujte terénní data v PageSpeed Insights nebo Search Console. Laboratorní zlepšení je jen hypotéza, dokud se nepotvrdí v reálných návštěvách.

## Co je v plném digitálním balíčku

- pracovní postup pro LCP, INP a CLS;
- tabulky pro terénní a laboratorní měření;
- rozhodovací strom pro obrázky, JavaScript, fonty, embed prvky, cache a rozvržení;
- šablona priorit pro vlastní tým a vývojáře;
- regresní checklist a 30denní plán;
- základní vysvětlení, kdy samotný návod nestačí a je potřeba výkonový audit.

Pro web, kde chcete výkon skutečně proměřit a provést základní optimalizaci, je k dispozici **výkonový audit + optimalizace od 12 600 Kč**. Výchozí rozsah, technické přístupy, závislosti na CMS/hostingu a termín se potvrzují před objednávkou.

## Zdroje

[1]: https://developers.google.com/search/docs/appearance/core-web-vitals "Google Search Central — Understanding Core Web Vitals and Google search results"
[2]: https://web.dev/articles/vitals-measurement-getting-started "web.dev — Getting started with measuring Web Vitals"
