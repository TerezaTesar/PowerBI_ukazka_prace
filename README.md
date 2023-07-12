# PowerBI_ukazka_prace
Projekt vznikl jako ukázka práce s daty pro společnost Cross Master, s jejím dovolením zveřejňuji


Na zadaných datech bylo úkolem vypracovat tři body.

   Úkol 1: 
	Na jaké kategorii produktů máme největší obrat? Mění se na tom v jednotlivých 	měsících něco?
Postup: 
    • Do tabulky Transactions jsem přidala sloupečky Category a Price per Quantity (násobek ceny produktu z tabulky Products a počtu kusů v objednávce). 
    • Přidala jsem součtové measury (SUM) na sloupci Price per Quantity pro výpočet obratu v jednotlivých kategoriích produktů.
    • Pomocí těchto součtů jsem vytvořila graf vývoje obratu v jednotlivých kategoriích produktů v závislosti na datu. Z Datové hierarchie jsem vybrala zobrazení po měsících.
    • Pro zobrazení jsem zvolila Area Chart, který přehledně zobrazuje vývoj ve všech kategoriích v jediném grafu.
       
Úkol 2:
	Který den v týdnu je nejsilnější na počet objednávek?
Postup:
    • U sloupce Transaction ID jsem změnila nastavení sčítání na Count (Distinct) což mi umožnilo sečíst pouze unikátní čísla objednávek jako SUM Transaction ID. 
    • Ze sloupce Date jsem si vykopírovala den v týdnu jako číslo a nahradila ho slovním označením (0 => Sunday, 1 => Monday, ...).
    • Pro zobrazení jsem zvolila Clustered Column Chart (seřazený od nejvyšší hodnoty po nejnižší), ze kterého je zřejmé, že v pondělí a o sobotách chodí nejvíce objednávek.

Úkol 3:
	Od 18. 3. 2022 došlo k navýšení budgetu na online marketingových platformách 	(Google Ads, Sklik, Facebook). Ovlivnilo to nějak prodeje? A pokud ano, tak jak? 	(externí vlivy zanedbejme)
Postup:
    • Pro zhodnocení vlivu navýšení budgetu na online marketingových platformách jsem použila SUM Transaction ID (Počet objednávek) a SUM Price per Quantity (Obrat) z předchozích úkolů.
    • Jako zobrazení Součtu počtu objednávek a Obratu jsem vybrala Clustered Column Chart seřazené časově po měsících a k tomu Line chart pro zobrazení počtu objednávek v jednotlivých dnech. Na liniovém grafu vynikají dny s vyšším počtem objednávek, zatím co sloupcové grafy ukazují kumulativní výkon objednávek a obratu v měsících.
