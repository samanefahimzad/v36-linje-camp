Peka på tavlan: selektorn där du satte display: grid (.tabla) — varför behövs rader och kolumner?

Rader och kolumner behövs för att bestämma hur elementen ska placeras och ordnas på sidan.

Peka på pärlbandet: selektorn med display: flex (.kort-rad) — varför räcker en riktning?
För att flex bara behöver ordna korten åt ett håll,


Peka på resultatet: beskriv vad som händer om du byter verktyg 
(Flex på tabla = en rad som kläms; Grid på kort = onödigt tungt för ett band).




Flex vs Grid

På min linje-sida använder jag display: grid på .tabla eftersom avgångarna behöver både rader och kolumner. 
Det passar bra för en avgångstavla med till exempel tider och spår.

På .kort-rad använder jag display: flex eftersom korten främst ska ligga bredvid varandra i en riktning. 
Det blir som ett pärlband och behöver därför inte ett helt rutnät.

Om jag skulle använda Flex på .tabla skulle innehållet försöka klämmas in på en rad. Om jag använder Grid på .kort-rad blir det mer komplicerat än vad som behövs.

Ägarskap

Jag kan förklara varje rad jag har pushat. AI är ett verktyg som hjälper mig att tänka, men det ersätter inte min egen förståelse av koden.


Varför sitter display: grid på .tabla och inte på varje .avgang?

För att .tabla ska styra hur alla .avgang placeras tillsammans i rader och kolumner. .avgang är bara själva innehållet.

Vad gör 1fr jämfört med att sätta width: 33% på varje cell?
1fr delar upp utrymmet jämnt mellan kolumnerna. width: 33% ger varje cell 33% av bredden, vilket kan bli problem med mellanrum (gap).


Vad händer om href="#tabla" pekar rätt men section saknar id="tabla"?
Då händer inget när man klickar på länken, eftersom det inte finns något element med id="tabla" att gå till.


Varför behöver tabla en media query men destinationer ofta klarar sig med flex-wrap?
För att .tabla har flera kolumner som kan bli trånga på en liten skärm. Därför behöver den ändras med en media query.

destinationer använder flex-wrap, så korten kan automatiskt flytta ner till nästa rad när det blir ont om plats.