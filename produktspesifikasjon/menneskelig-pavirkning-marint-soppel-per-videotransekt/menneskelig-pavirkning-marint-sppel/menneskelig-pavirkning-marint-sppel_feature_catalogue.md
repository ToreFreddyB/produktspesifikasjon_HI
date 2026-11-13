#### MarintSøppelVideotransekt

Navnet på platformen som ble brukt til videofilming.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>posisjon</td>
      <td>sted som objektet eksisterer på.<br />Location where the object exists</td>
      <td>GM_<wbr />Point</td>
      <td>1</td>
    </tr>
    <tr>
      <td>marine<wbr />Grunnkart<wbr />Id</td>
      <td>Unikt fortløpende id-nummer i Marine grunnkart.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>plattform</td>
      <td>Fartøy som har innhentet data.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>region</td>
      <td>Regionen som videotransektet er tatt i. Samsvarer med lokalitetene i Marine grunnkart.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>tokt<wbr />Nummer</td>
      <td>toktnummer ved Havforskningsinstituttet.<br />-- Definition --<br />Cruise number at IMR.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>stasjon<wbr />Id</td>
      <td>Unik Stasjons-ID for videotransektet (samsvar med navn på videofilm).</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>lengde<wbr />Transekt</td>
      <td>Lengde på transekt (f.eks 50 m).</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>lengdegrad</td>
      <td>Lengdegrad (midt lengdegrad for transektet)</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>breddegrad</td>
      <td>Breddegrad (midt breddegrad for transektet)</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>presisjon</td>
      <td>Presisjon (fra-til, f.eks. 10-100 m).</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>startdato</td>
      <td>Dato (angitt ved starten på transektet).</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>dyp1</td>
      <td>Dyp ved start på transekt</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>dyp2</td>
      <td>Dyp ved slutt på transekt.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>dyp<wbr />Type</td>
      <td>Beskriver dyp1 og dyp2 med en av tre mulige egenskaper: Dyp på midten, Gjennomsnittlig dyp, eller Start-slutt dyp.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>søppel<wbr />Dekning</td>
      <td>Beskriver om det er observert søppel på dette videotransektet. Kan ha verdiene: Masse søppel. Søppel tilstede. Ingen søppel.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>søppel<wbr />Mengde</td>
      <td>Verdi for totalt antall søppelobservasjoner på videotransektet (sum av de ulike kategoriene).</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>diverse<wbr />Avfall</td>
      <td>Antall observasjoner av uidentifiserbart avfall på videotransektet.<br />Heltall.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>glass<wbr />Keramikk</td>
      <td>Antall observasjoner av glass, keramikk o.l. på videotransektet.<br />Heltall.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>gummi</td>
      <td>Antall observasjoner av gummi i videotransektet.<br />Heltall.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>metall</td>
      <td>Antall observasjoner av metall på videotransektet.<br />Heltall.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>naturlige<wbr />Produkter</td>
      <td>Antall observasjoner av naturlige produkter (tøy, tre o.l.) videotransektet.<br />Heltall.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>plast</td>
      <td>Antall observasjoner av plast på videotransektet.<br />Heltall.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>sanitær<wbr />Avfall</td>
      <td>Antall observasjoner av sanitært avfall på videotransektet.<br />Heltall.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>marint<wbr />Søppel<wbr />Kommentar</td>
      <td>Beskriver mer detaljert de ulike søppelobservasjonene på videotransektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaperMarintSøppelVideotransekt</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>unik identifikasjon av et objekt</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br /><br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br /><br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br /><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>beskrivelse av kvaliteten på stedfestingen<br />Merknad: Denne er identisk med ..KVALITET i tidligere versjoner av SOSI.</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- målemetode</td>
      <td>metode for måling i grunnriss (x,y), og høyde (z) når metoden er den samme som ved måling i grunnriss</td>
      <td><a href="#kodeliste-målemetode">Målemetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>datauttaksdato</td>
      <td>dato for uttak fra en database<br />Merknad:<br />Skiller seg fra Kopidato ved at en ikke skiller på om det er uttak fra en originaldatabase eller en kopidatabase.</td>
      <td>Date<wbr />Time</td>
      <td>1</td>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning<br /><br />Merknad:<br />mulighet til å legge inn utfyllende informasjon om objektet</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>opphav</td>
      <td>referanse til opphavsmaterialet, kildematerialet, organisasjons/publiseringskilde<br />Merknad:<br />Kan også beskrive navn på person og årsak til oppdatering</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
GenerelleEgenskaperMarintSøppelVideotransekt

#### GenerelleEgenskaperMarintSøppelVideotransekt (abstrakt)

abstrakt objekt som bærer en rekke egenskaper som er fagområde-uavhengige og kan benyttes for alle objekttyper<br />Merknad: Spesielt i produktspesifikasjonsarbeid vil en velge egenskaper og av grensningslinjer fra denne klassen.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>identifikasjon</td>
      <td>unik identifikasjon av et objekt</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br /><br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br /><br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br /><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>beskrivelse av kvaliteten på stedfestingen<br />Merknad: Denne er identisk med ..KVALITET i tidligere versjoner av SOSI.</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- målemetode</td>
      <td>metode for måling i grunnriss (x,y), og høyde (z) når metoden er den samme som ved måling i grunnriss</td>
      <td><a href="#kodeliste-målemetode">Målemetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>datauttaksdato</td>
      <td>dato for uttak fra en database<br />Merknad:<br />Skiller seg fra Kopidato ved at en ikke skiller på om det er uttak fra en originaldatabase eller en kopidatabase.</td>
      <td>Date<wbr />Time</td>
      <td>1</td>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning<br /><br />Merknad:<br />mulighet til å legge inn utfyllende informasjon om objektet</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>opphav</td>
      <td>referanse til opphavsmaterialet, kildematerialet, organisasjons/publiseringskilde<br />Merknad:<br />Kan også beskrive navn på person og årsak til oppdatering</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
  </tbody>
</table>

### Kodelister

#### <a id="kodeliste-målemetode"></a>«CodeList» Målemetode

**Definisjon:** metode som ligger til grunn for registrering av posisjon


-- Definition - -
method on which registration of position is based

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="http://skjema.geonorge.no/SOSI/generelleKonsepter/generelleTyper/5.1/Målemetode">http://skjema.geonorge.no/SOSI/generelleKonsepter/generelleTyper/5.1/Målemetode</a></td>
    </tr>
  </tbody>
</table>
