# Resell Assistant — bezmaksas mobilās tīmekļa lietotnes prototips

## Kāpēc iepriekšējais HTML varēja nestrādāt?
iPhone lietotnes Files priekšskatījums var parādīt HTML, bet neizpildīt JavaScript. Šī lietotne ir paredzēta atvēršanai kā tīmekļa lapa, izmantojot HTTPS. Kad tā publicēta HTTPS adresē, vari to pievienot iPhone sākuma ekrānam un izmantot kā vienkāršu PWA.

## Publicēšana bez maksas ar GitHub Pages
1. Izveido vai pieslēdzies GitHub kontam.
2. Izveido jaunu publisku repozitoriju, piemēram, `resell-assistant`.
3. Augšupielādē repozitorijā `index.html`, `manifest.webmanifest` un `sw.js` no šīs mapes.
4. Repozitorijā atver **Settings → Pages**.
5. Pie **Build and deployment** izvēlies **Deploy from a branch**, zaru `main` un mapi `/(root)`, tad spied **Save**.
6. Pagaidi, līdz GitHub Pages parāda publicēto HTTPS saiti.
7. Atver saiti Safari iPhone. Spied **Share → Add to Home Screen**. Izvēlies **Open as Web App**, ja šāda izvēle tiek piedāvāta.
8. Pievieno testa preci un pārbaudi, vai tā saglabājas pēc lapas aizvēršanas un atkārtotas atvēršanas.

## Funkcijas
- Preču katalogs un statusi 20–100+ precēm (atkarīgs no foto un pārlūka krātuves).
- Fotoattēlu samazināšana pirms saglabāšanas.
- Pašizmaksas, plānotās cenas un realizētās peļņas aprēķins.
- Sludinājuma melnraksta ģenerēšana un kopēšana.
- Atbilžu šabloni.
- Meklēšana, filtrēšana, rediģēšana, dzēšana.
- JSON rezerves kopija ar fotogrāfijām un CSV eksportēšana.
- Pamata offline kešošana pēc pirmās ielādes.

## Datu glabāšana
Dati glabājas pārlūkprogrammas `localStorage` šajā ierīcē. Nav lietotāja konta, mākoņa sinhronizācijas vai servera datubāzes. Regulāri eksportē JSON rezerves kopiju. Nelieto privātā pārlūkošanas režīmu.

## Ierobežojumi
- Šis nav Vinted produkts un nepieslēdzas Vinted API.
- Tas automātiski nepublicē sludinājumus, nesūta pircējiem ziņas un neapstrādā pasūtījumus.
- Vinted API izmanto tikai tad, ja Vinted tev piešķir oficiālu piekļuvi un tavs pārdošanas modelis ir atļauts Latvijā.
- GitHub Pages ir bezmaksas statiskai vietnei, bet publiskā repozitorijā avota kods ir publiski redzams. Šajā prototipā nav ievadāmu kontu paroļu vai API atslēgu.
