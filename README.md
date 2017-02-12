## Stránky

Každá stránka je samostatný soubor s příponou ".md". Výsledná adresa, na kterou se jde v prohlížeči, je název soubor bez přípony. Několik příkladů:

  1. Soubor `foo.md` vytvoří stránku http://www.ctyridvory-vysocina.cz/foo.
  2. Soubor `ubytovani/cenik.md` vytvoří stránku http://www.ctyridvory-vysocina.cz/ubytovani/cenik.

Několik důležitých poznámek:

  1. Homepage (http://www.ctyridvory-vysocina.cz/) se nachází v soubor `index.md`, a nemůže tomu být jinak.
  2. Pokud by stránka měla mít mezery v názvu, je třeba je nahradit pomlčkami ("volné pokoje" => `volne-pokoje.md`).





## Metainformace o stránce

Obsah každé stránky musí začínat zvláštním blokem:

```
---
description: ...
layout: default
title: ...
---
```

Několik důležitých poznámek:

  1. Před blokem nesmí být žádné mezery ani volné řádky.
  2. Na konci řádků nesmí být žádné mezery.
  3. Řádek s `layout: default` musí zůstat tak, jak je.
  4. Všechny jiné řádky kromě těchto tří musí zůstat tak, jak jsou.





## `title` a `description` ve zvláštním bloku

Ideálně by každá stránky měla mít `title` i `description` vyplněný. `description` je možné vynechat, ale nedoporučuji to. Čím více poctivě vyplněného obsahu, tím lépe.

  1. `title` by měl mít následující podobu (pomlčka odděluje "úrovně" webu):

    1. Čtyři Dvory Vysočina
    2. Ubytování - Čtyři Dvory Vysočina
    3. Volné pokoje - Ubytování - Čtyři Dvory Vysočina

  2. `description` se zobrazuje u položky ve výsledcích vyhledávání Google, takže by to měl být lidsky srozumitelný text, něco co zaujme.





## Formátování obsahu stránek

Zbytek souboru `.md` je vlastní obsah stránky. Platí pro něj následující formátovací pravidla:

  1. Odstavec textu je každý shluk textu oddělený od zbytku volným řádkem nahoře a dole.
  2. Slovo nebo větu lze zvýraznit pomocí hvězdiček: `**tučné slovo**` a `*slovo kurzívou*`.





## Formátování: nadpisy

Lze vytvářet nadpis od 1. až do 6. úrovně. Nadpis se vytvoří přidáním křížku (`#`) na začátek řádku.

```
# Toto je nadpis 1. úrovně
```

```
## Toto je nadpis 2. úrovně atd.
```

Pro nadpis platí důležitá poznámka:

  1. Kolem nadpisu musí být volné řádky. Následující příklad je **špatně**:

     ```
     # Toto je špatně vytvořený
     # nadpis na dvou řádcích
     ```





## Odkazování se na další stránky

Odkaz na jinou stránku lze vytvořit pomocí následujícího zápisu:

```
[toto je odkaz do fotogalerie](/fotky)
```

Část ve hranatých závorkách je to, co uvidí uživatelé. Část v kulatých závorkách je to, kam se dostanou po kliknutí na odkaz.
