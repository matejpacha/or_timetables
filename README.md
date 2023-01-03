# or_timetables
This project contains my Timetables for OpenRails. Since the route is situated in Czechia, the rest of the text, supporting materials and descriptions are in Czech. Should you have any questions, please leave a message.

# Popis
Projekt obsahuje "jízdní řády" aneb "Timetable mode" soubory pro Openrails CZSK na trati BP primárně v úseku Jihlava - Havlíčkův Brod. Jízdní řád je inspirovaný GVD 2005/2006, jehož sešitové jízdní řády jsou součástí souborové struktury.

## Co od toho čekat?
Nic. Timetable mode je nuda. Jezdíte podle jízdních řádů a není moc prostoru na změny. Je to rutina. Některé "postižené" jedince to ale baví, takže ti jsou vítáni. Některé služby mají prostoje i hodinu (podobně jako v reálu), takže doporučuji si procvičit zrychlení času (ale ne více jak na cca 500%, potom TT nedokáže simulovat správně a dochází ke zpožděním nebo i neschopnostem rozjet se ze stanice/zastávky). Důležité: nejedná se o kompletní GVD a už vůbec ne o věrný GVD. Pokud máte jiné zkušenosti, vzpomínky či přímo důkazy (technologické postupy, fotky, videa z té doby), pak vězte, že máte pravdu.
TT stavím tak, aby si žil svým vlastním životem. V Jihlavě a v HavlBrodě mám zálohy, které lze využít na prosté pozorování. Vlaky označené "standardně" jsou určené pro hráče. Vlaky označené podtržníkem (např. "_R667") jsou spíše nutností pro provoz (tedy např. vlak _R667 začíná na trati mezi Jihlavou-Městem a hráč by tedy jen dovezl vlak k nástupišti a odstavil lokomotivu - nic záživného).

## Proč zrovna Jihlava-Havlíčkův Brod?
Jihlava je rodné město mé. A protože jsem na internetu našel sešiťáky pro GVD 2005/6, používám je jako zdroj provozu. Nemám jiné zdroje. Technologické postupy (lze-li to tak nazvat) jsou kombinací mé chatrné paměti a možností samotného TT. Ne všechny postupy je možné realizovat podle předlohy - už jen kvůli návěstnímu systému tratě BP a jeho zpracováním v OR, případně kvůli omezené sadě manipulací v TT. Každopádně je GVD2005/2006 na trati BP v95+ silně neautentický - pan Šemora se zaměřil na období již zprovozněného autobloku mezi Jihlavou a HavlBrodem, nicméně v roce 2006 ještě autoblok dokončen nebyl a bylo to zároveň období častých výluk (viz např. http://spz.logout.cz/novinky/novinky.php?poradi=995). Berte to tedy prosím jen jako inspiraci reálným provozem, který byl nicméně aspoň v Jihlavě zajímavý svou pestrostí. Rychlíky Brno - Č.Budějovice si předávaly plecháče (laminátky) s brejlovci, na motorácích se střídaly 850 s 843, bylo vidět poměrně dost vlaků na relaci Maloměřice - Budějovice (uhlí do Rakouska) a do toho pendlují laminátky s patrem a hitlákem, občas střídané motoráčkem. Srdcovkou byl pak rušící R1518/1519, který si dovolím implementovat ještě s řadou 749, jejíž dunění provázelo mé dospívání. Snažím se do provozu dávat i související relace a oživit tak aspoň stanice Havlíčkův Brod nebo Okříšky (zatím v plánu). Delší trasy (např. do Brna) se asi taky vyskytnou, ale nebude to nic pravidelného (zatěžuje to spouštění OpenRails).

## Co k tomu potřebujete?
- [Openrails CZSK](https://msts-rw.cz/openrails-icik-cz-sk-verzia/) - v tom testuji. Pokud někdo používá klasiku nebo MG, neručím za funkčnost (ostatně já neručím za nic)
- [Trať BP](https://semora.cz/msts/) v poslední aktualizaci, minimálně ale v95.00
- Trainset BP + pravděpodobně něco navíc, případně editor consistů, kde si napasujete vozidla a soupravy podle sebe
- Nervy
- Případně program [Grafikon ve verzi 4.1](https://github.com/jub77/grafikon/releases) (moje pomůcka pro tvorbu), Adobe Reader (nebo ekvivalent), Microsoft Excel (verze 365)

## Kdy se dočkáte kompletního TT?
Na základě zkušeností z jiných podobných projektů i jiných autorů: nikdy. Ale zatím mě to baví, takže občas udělám aktualizaci (dostupná na GITu). Doporučuji nainstalovat si klienta Gitu a provádět "pull" operace, případně pokud sami do tvorby zasáhnete, tak "fetch". Není to ale nic nutného.

## Můžete pomoci?
Ano - stačí mi napsat, že máte zájem. Ať už jako testeři, anebo jako přispěvatelé - můžete tvořit TT, dávat dohromady trasy, consisty, modely a skiny, dynamickým počasím, atd. Anebo jenom tím, že tento svérázný projekt nezahrabete pod černou zem. Případně radou, pokud už máte v TT něco za sebou. Jo a nekonstruktivní kritiku si nechejte pro sebe. Na hejty už jsem starej.

## Poznámka:
Opustil jsem Openrails Timetable Editor, protože neumožňuje slušnou práci s tabulkami. Takže nastoupil Excel postavený čistě na vzorcích. Obsahuje pouze jedno makro, které ukládá výsledný soubor. Šikovní si jistě upraví podle potřeby, nešikovní můžou makra zakázat a používat Ctrl+C/Ctrl+V s následnou úpravou do formátu odděleného ";" (ale neručím za funkčnost ručního postupu - např. v briefingu se může objevit čárka a její následné nahrazení středníkem udělá v timetable paseku. Proto je Makro lepší, ale musíte mu "věřit").
A sdílený obsah používejte dle uvážení. Pokud by vás nedejbože napadlo zveřejnit vlastní klon tohoto TT, potěší mě poděkování.

## Stručný troubleshooting:
- OR nevidí Timetable: zkontrolujte umístění souboru
- Při spuštění OR skončí s chybou: Přečtěte si chybovou hlášku a postupujte přiměřeně jejímu znění. Pokud z ní nejste moudří, otevřete si soubor OpenRailsLog.txt na ploše - hledejte někde na konci. Pokud ani z toho nejste moudří, hledejte chyby v consistech - chybějící vozidla, atd.
- Při jízdě došlo ke konfliktu (jízda proti druhému vlaku, nevybavené návěstidlo, atd.) - zkuste se na GitHubu vrátit o jednu verzi zpět, případně podle logu zkuste dohledat změny týkající se vašeho vlaku a jízdu opakujte. Aktualizací mohlo dojít k narušení provozu jiného vlaku.


