Wordle jolasa

HTML, CSS eta JavaScript erabiliz egindako Wordle motako jolasa.

Nola jolastu
Aukeratu saiakera kopurua eta hitzaren letra kopurua, eta sakatu Jugar botoia.
Idatzi letrak teklatu birtualarekin edo benetako teklatuarekin:
Enter: saiakera bidali.
Backspace / Supr: azken letra ezabatu.
Koloreak:
Berdea (ok): letra ondo kokatuta dago.
Horia (existe): letra hitzean dago, baina beste lekuan.
Grisa (no): letra ez dago hitzean.
Jolasa amaitzen da hitza asmatzen denean edo saiakerak agortzen direnean. Orduan, azken 10 jolasen zerrenda erakusten da, eta berriro jolasteko botoia.
Fitxategiak
Fitxategia	Zertarako
wordle.html	Orriaren egitura: formularioa, taula, teklatua eta historiala.
styles.css	Estiloak: Grid, Flexbox eta koloreentzako aldagaiak.
javawordle.js	Jolasaren logika.
API

Hitza lortzeko fetch bat egiten da hurrengo APIra:

https://words-api-sy2x.onrender.com/api/word?lang=es&length=5&number=1
lang: hizkuntza (es edo eu).
length: hitzaren luzera (3 baino handiagoa).
number: itzuli beharreko hitz kopurua.

APIak hitzak tildeekin itzul ditzake; programak tildeak kentzen ditu (Ñ letra mantenduz), teklatuan tilderik gabeko letrak bakarrik daudelako.

localStorage

Jolas bakoitza wordleHistorial gakoan gordetzen da, objektuen zerrenda gisa (azken 10 jolasak bakarrik):

json
{
  "palabra": "CASAS",
  "intentos": ["MESAS", "CASAS"],
  "fecha": "11/10/2026, 18:30:00",
  "resultado": "ganada"
}
palabra: asmatu behar zen hitza.
intentos: egindako saiakerak.
fecha: jolasaren data eta ordua.
resultado: ganada edo perdida.
Erabilitako teknologiak
HTML5
CSS3 (Grid, Flexbox eta aldagaiak)
JavaScript (fetch, async/await, gezi-funtzioak, localStorage)
