# Recepty z kuchyně (receptyzkuchyne.cz)

Veřejný web s recepty. Jeden statický soubor `index.html`, nic se nesestavuje.

## Jak to funguje
- Recepty a jídla se na web dostávají z aplikace **Mise** tlačítkem „Zveřejnit na web" (u receptu nebo jídla).
- Web si je načítá v prohlížeči z databáze Mise (Supabase, tabulka `web_posts`) veřejným klíčem, který umí jen číst.
- Pořadí a mazání příspěvků: v Mise na stránce „Web příspěvky" (jen správce).

## Nasazení
- Hosting: Vercel, projekt `recepty-web`, domény www.receptyzkuchyne.cz a receptyzkuchyne.cz.
- Každá změna ve větvi `main` se na Vercelu nasadí sama (zhruba do minuty).

## Historie
- 24. 6. 2026 — web nasazen ručně (`vercel deploy`), bez gitu.
- 11. 9. 2026 — přesná kopie produkce uložena sem, Vercel napojen na toto repo.
