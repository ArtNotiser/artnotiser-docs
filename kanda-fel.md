# Kända fel i ArtNotiser

Nedan finns en lista över kända fel i ArtNotiser, det inkluderar både fel i analysprocessen, i epost-utskicken och i mobilappen.

## När jag själv rapporterar ett kryss så får jag notis om att det är ett nytt kryss
<i>Skapad: 2023-01-19</i>

Felet uppstår när du rapporterar ett nytt årskryss och din notis genereras innan krysslistorna uppdateras. Detta är ett temporärt problem som löser sig när krysslistorna uppdaterats, vilket sker var 6:e timme.

## Jag ser "svanar" och "gäss" i mina notiser
<i>Skapad: 2023-01-19</i>

Detta orsakas av att rapportören har använt sig av en obestämd art, tex "Ob. svan", vilket översätts till "svanar" när ArtNotiser läser från Artportalen. Eftersom du som användare inte har "svanar" eller "gäss" på din årslista så tror ArtNotiser att det är ett nytt årskryss för dig.

Vi kommer framöver undersöka om `dyntaxaTaxonId`eller `taxonCategory` kan användas för att lösa problemet.