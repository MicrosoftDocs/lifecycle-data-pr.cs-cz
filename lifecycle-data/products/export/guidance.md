---
title: Průvodce exportem dat životního cyklu
description: Průvodce exportem informací o životním cyklu produktu
ms.date: 12/16/2020
layout: ContentPage
ms.openlocfilehash: 5e9dddbff5fac32e6d3cf8ef0943151d2dfe5e35
ms.sourcegitcommit: 6ea3221fd5475440480515f04f33988656d71748
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/02/2021
ms.locfileid: "3546764"
---
# <a name="lifecycle-data-export-guidance"></a>Průvodce exportem dat životního cyklu
Tento dokument popisuje, jak použít soubor exportu produktu.

## <a name="query-information"></a>Informace dotazů
V programu Excel jsou pole, která pomáhají identifikovat data vyplněná v tabulce produktů.

### <a name="end-of-support"></a>Konec podpory
Hodnota konce podpory bude filtrovat produkty podle data ukončení podpory produktu nebo podle data ukončení jeho vydání.

Možné hodnoty: Vše (není použit žádný filtr), Rok a Oblast.

### <a name="family"></a>Rodina
Hodnota rodiny filtruje produkty podle nadřazené úrovně v hierarchii označované jako rodina.

Možné hodnoty: Vše (není použit žádný filtr), Název rodiny

### <a name="group"></a>Skupina
Hodnota skupiny filtruje produkty v rámci nadřazené úrovně (rodiny) do určité skupiny.

Možné hodnoty: Vše (není použit žádný filtr), Název skupiny

## <a name="table-columns"></a>Sloupce tabulky
Tabulku produktů tvoří sloupce definující produkt, edice, verze a odpovídající data podpory.

> [!NOTE]
> Pro každý produkt, edici a kombinaci verzí bude řádek.

### <a name="product"></a>Produkt
Název produktu.

### <a name="edition"></a>Vydání
Sloupec vydání se vyplní, když produkt obsahuje vydání. Pokud není žádné vydání produktu, bude toto pole prázdné.

### <a name="release"></a>Release
Sloupec verze se vyplní, když produkt obsahuje více verzí.
Pokud má produkt jenom jednu verzi, bude toto pole prázdné.

### <a name="support-policy"></a>Zásady podpory
Toto pole definuje zásady podpory, které produkt sleduje.

Možné hodnoty: [Pevné](/lifecycle/policies/fixed), [Moderní](/lifecycle/policies/modern), Komponenta

### <a name="start-date"></a>Počáteční datum životního cyklu
Pro produkt byla zahájena podpora od data.

### <a name="mainstream-date"></a>Hlavní datum
Pokud je zásada podpory **pevná** nebo **komponenta**, jedná se o datum hlavního data ukončení produktu.
  
Pokud je zásada podpory **moderní,** bude tato zásada prázdná.

### <a name="extended-end-date"></a>Datum ukončení rozšířené podpory
Pokud je zásada podpory **pevná** nebo **komponenta**, je to datum rozšířeného koncového data produktu.

Pokud je zásada podpory **moderní,** bude tato zásada prázdná.

### <a name="retirement-date"></a>Datum vyřazení
Pokud je zásada podpory **pevná** nebo **komponenta**, bude tato zásada prázdná.

Pokud jsou zásady podpory **moderní,** bude to datum vyřazení produktu.

### <a name="release-start-date"></a>Počáteční datum životního cyklu
Pro vydání byla zahájena podpora pro datum. Pokud má produkt jenom jednu verzi, bude toto pole prázdné.
 
### <a name="release-end-date"></a>Datum ukončení vydání
Datum ukončení podpory pro vydání
Pokud má produkt jenom jednu verzi, bude toto pole prázdné.

### <a name="docs-url"></a>Docs Url
Adresa URL rozšířené dokumentace
