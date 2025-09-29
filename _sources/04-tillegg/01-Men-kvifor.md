# Men, Andreas, kvifor?

([In English](/04-tillegg/02-But-why.md))

Forfattar Cory Doctorow er aktivist for kulturdeling, og gir alle bøkene sine ut med opne lisensar sidan 2003 – det er ei politisk avgjerd som også gjev han «kunstnarleg, moralsk og kommersiell tilfredsstilling», men også noko han meiner fører til auka salg og spreiing av bøkene sine.

Boka "Little Brother" tidlegare gitt ut på nynorsk frå Samlaget som "Veslebror ser deg" i 2009. Boka er vel omsett av Øystein Vidnes, som gav han Kulturdepartementets Oversetterprisen same året. 

 I motsetning til enkelte andre utgivingar i andre land vart ikkje Samlaget si omsetjing lagt ut med Creative Commons-lisensar – dei gav likevel først ut halve boka gratis på nett på  [veslebrorserdeg.com](https://web.archive.org/web/20100104043824/http://www.veslebrorserdeg.com)(Wayback Machine-lenke frå tidleg 2010), og resten kun på direkte oppfordring, før dei etter press frå forfattaren og nørds i Noreg gav ut heile boka gratis.

Men det tok ikkje lang tid før domenet døydde ut, og tilgangen til boka vart vekke – og i dag er einaste måten å få lest boka å låne den gjennom ei biblioteksteneste, å kjøpe den brukt, eller å få tilsendt PDF-fila frå ein anna fan. Eg vert glad når kultur meint for å vere i det fri får vere i det fri, og irriterte meg veldig då den norske omsetjinga sitt digitale fotavtrykk vart vekke.

Domenet veslebrorserdeg.com var tilgjengeleg, så eg kjøpte det. Eg ynskja å gjere boka elektronisk fritt tilgjengeleg igjen, men eg turte ikkje å legge ut Samlaget sin PDF. I samtale med Thomas Brevik vart eg påmint at Creative Commons-lisensen tillét bearbeida verk, som omsetjingar, så lenge dei er gitt ut under same lisens.

Så [[02-intro|dette er mi omsetjing]], dels støtta av maskinlæring med meg som redaktør og finlesar. Den er ikkje like god som Vidnes si, men den finst, og er fritt tilgjengeleg, og er lagt ut under same lisens som originalen. Om Samlaget ynskjer å få den opphavlege omsetjinga si ut i verda, så stiller eg meg tilgjengeleg for å legge den ut her.

"Little Brother" er ein heilt greit underhaldande pageturner med nørdete forteikn. Men det eg synest den gjer best, er å – allereie før overvåkingskapitalismen tok heilt av – vere ei snøgginnføring i arbeid mot undertrykking i ei stadig meir digitalisert verd, og den er stadig lynande aktuell, truleg endå meir no enn då den kom ut.

Som Doctorow sjølv skriv i [introduksjonen](/01-intro/02-intro.md): 

> **"Denne boka er meint å vere noko du *gjer*, ikkje berre noko du les."**

## Men, Andreas, korleis?
Dette er fullstendig ukommersiell business. Om du vil gi nokon pengar, kjøp ei av Doctorow sine bøker i staden, eller [sjekk om du kan donere eksemplar av boka til lærarar eller andre trengande](https://craphound.com/littlebrother/donate/). Forlaget Kvefsebol er noko eg har tenkt skulle vere eit namn til om eg publiserte noko rollespelinnhald på nett, men sidan det aldri materialiserte seg, så blei det her i staden.

Sida er bygd opp av ei rekke markdown-filer som eg har forsøkt etter beste evne å finlese. Ved hjelp av systemet [JupyterBook](https://jupyterbook.org/en/stable/start/build.html) har eg så laga søkbare HTML-sider av filene, og publisert dei på [Github](https://github.com/tanketom/veslebrorserdeg).

Når eg no oppdaterer ei markdown-file, så går eg til Terminal, opnar foreldremappa til prosjektet, og taster:

```
jupyter-book build veslebrorserdeg/
```

Så 

```
cd veslebrorserdeg
ghp-import -n -p -f _build/html
```

Så tek Github seg av resten!