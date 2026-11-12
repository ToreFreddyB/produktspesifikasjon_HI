#### GrabbPrøver

Prøver som er samlet inn med grab.<br />Samples collected by the use of grab.

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
      <td>sted som objektet eksisterer på.<br />Location where the object exists.</td>
      <td>Punkt</td>
      <td>1</td>
    </tr>
    <tr>
      <td>redskap</td>
      <td>type redskap benyttet for prøvetakingen.<br />Name of equipment used for the sampling.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>arter<wbr />Enhet</td>
      <td>enhet for antall arter.<br />Unit used for number of species.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>biomasse<wbr />Enhet</td>
      <td>enhet benyttet for biomasse for det aktuelle redskapet.<br />Unit used for weigth for this equipment.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>individer<wbr />Enhet</td>
      <td>enhet benyttet for individer for det aktuelle redskapet.<br />Unit used for number of individuals for this equipment.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesEgenskaperPrøver</th>
    </tr>
    <tr>
      <td>referanse<wbr />Stasjon</td>
      <td>referansestasjon, unik innen MAREANO.<br />Reference number during MAREANO prosject (superstation).</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>tokt<wbr />Nummer</td>
      <td>toktnummer ved Havforskningsinstituttet.<br />Cruise number at IMR.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>arter</td>
      <td>antall forskjellige arter funnet i prøven.<br />Nos different species in the sample.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>individer</td>
      <td>individer funnet i prøven.<br />Individuals in the sample.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>biomasse<wbr />Vekt</td>
      <td>biomasse av arter funnet i prøven.<br />Weight of individuals in sample.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>lengdegrad</td>
      <td>lengdegrad som prøven ble tatt på.<br />Longitude where the sample was taken.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>breddegrad</td>
      <td>breddegrad som prøven ble tatt på.<br />Latitude where the sample was taken.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>bunndyp</td>
      <td>bunndyp der prøven er tatt.<br />Bottomdepth where the sample is taken.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaperPrøver</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>unik identifikasjon av et objekt</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator, tildelt av dataleverendør/dataforvalter. Den lokale identifikatoren er unik innenfor navnerommet, ingen andre objekter har samme identifikator.<br />NOTE: Det er data leverendørens ansvar å sørge for at denne lokale identifikatoren er unik innenfor navnerommet.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til objektet, starter med to bokstavs kode jfr ISO 3166. Benytter understreking  ("_") dersom data produsenten ikke er assosiert med bare et land.<br />NOTE 1 : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og vil registreres i "INSPIRE external  Object Identifier Namespaces Register"<br />Eksempel: NO for Norge.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen.<br />NOTE Maksimum lengde er valgt for å tillate tidsregistrering i henhold til  ISO 8601, slik som  "2007-02-12T12:12:12+05:30" som versjonId.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>beskrivelse av kvaliteten på stedfestingen<br />Merknad: Denne er identisk med ..KVALITET i tidligere versjoner av SOSI.</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>0..1</td>
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
      <td>0..1</td>
    </tr>
    <tr>
      <td>første<wbr />Datafangstdato</td>
      <td>dato når data ble registrert/observert/målt første gang, som utgangspunkt for første digitalisering<br /><br />Merknad:<br />førsteDatafangstdato brukes hvis det er av interesse å forvalte informasjon om når en ble klar over objektet. Dette kan for eksempel gjelde datoen for første flybilde som var utgangspunkt for registrering i en database.</td>
      <td>Date<wbr />Time</td>
      <td>1</td>
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
FellesEgenskaperPrøver

#### FellesEgenskaperPrøver (abstrakt)

abstrakt objekt som bærer en rekke egenskaper som er felles for de tre objekttypene som realiseres i datasettet.

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
      <td>referanse<wbr />Stasjon</td>
      <td>referansestasjon, unik innen MAREANO.<br />Reference number during MAREANO prosject (superstation).</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>tokt<wbr />Nummer</td>
      <td>toktnummer ved Havforskningsinstituttet.<br />Cruise number at IMR.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>arter</td>
      <td>antall forskjellige arter funnet i prøven.<br />Nos different species in the sample.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>individer</td>
      <td>individer funnet i prøven.<br />Individuals in the sample.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>biomasse<wbr />Vekt</td>
      <td>biomasse av arter funnet i prøven.<br />Weight of individuals in sample.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>lengdegrad</td>
      <td>lengdegrad som prøven ble tatt på.<br />Longitude where the sample was taken.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>breddegrad</td>
      <td>breddegrad som prøven ble tatt på.<br />Latitude where the sample was taken.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>bunndyp</td>
      <td>bunndyp der prøven er tatt.<br />Bottomdepth where the sample is taken.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaperPrøver</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>unik identifikasjon av et objekt</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator, tildelt av dataleverendør/dataforvalter. Den lokale identifikatoren er unik innenfor navnerommet, ingen andre objekter har samme identifikator.<br />NOTE: Det er data leverendørens ansvar å sørge for at denne lokale identifikatoren er unik innenfor navnerommet.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til objektet, starter med to bokstavs kode jfr ISO 3166. Benytter understreking  ("_") dersom data produsenten ikke er assosiert med bare et land.<br />NOTE 1 : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og vil registreres i "INSPIRE external  Object Identifier Namespaces Register"<br />Eksempel: NO for Norge.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen.<br />NOTE Maksimum lengde er valgt for å tillate tidsregistrering i henhold til  ISO 8601, slik som  "2007-02-12T12:12:12+05:30" som versjonId.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>beskrivelse av kvaliteten på stedfestingen<br />Merknad: Denne er identisk med ..KVALITET i tidligere versjoner av SOSI.</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>0..1</td>
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
      <td>0..1</td>
    </tr>
    <tr>
      <td>første<wbr />Datafangstdato</td>
      <td>dato når data ble registrert/observert/målt første gang, som utgangspunkt for første digitalisering<br /><br />Merknad:<br />førsteDatafangstdato brukes hvis det er av interesse å forvalte informasjon om når en ble klar over objektet. Dette kan for eksempel gjelde datoen for første flybilde som var utgangspunkt for registrering i en database.</td>
      <td>Date<wbr />Time</td>
      <td>1</td>
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
GenerelleEgenskaperPrøver

#### BomtrålPrøver

Prøver som er samlet inn med bomtrål.<br />Samples collected by the use of beamtrawl.

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
      <td>sted som objektet eksisterer på.<br />Location where the object exists.</td>
      <td>Punkt</td>
      <td>1</td>
    </tr>
    <tr>
      <td>redskap</td>
      <td>type redskap benyttet for prøvetakingen.<br />Name of equipment used for the sampling.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>arter<wbr />Enhet</td>
      <td>enhet for antall arter.<br />Unit used for number of species.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>biomasse<wbr />Enhet</td>
      <td>enhet benyttet for biomasse for det aktuelle redskapet.<br />Unit used for weigth for this equipment.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>individer<wbr />Enhet</td>
      <td>enhet benyttet for individer for det aktuelle redskapet.<br />Unit used for number of individuals for this equipment.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesEgenskaperPrøver</th>
    </tr>
    <tr>
      <td>referanse<wbr />Stasjon</td>
      <td>referansestasjon, unik innen MAREANO.<br />Reference number during MAREANO prosject (superstation).</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>tokt<wbr />Nummer</td>
      <td>toktnummer ved Havforskningsinstituttet.<br />Cruise number at IMR.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>arter</td>
      <td>antall forskjellige arter funnet i prøven.<br />Nos different species in the sample.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>individer</td>
      <td>individer funnet i prøven.<br />Individuals in the sample.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>biomasse<wbr />Vekt</td>
      <td>biomasse av arter funnet i prøven.<br />Weight of individuals in sample.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>lengdegrad</td>
      <td>lengdegrad som prøven ble tatt på.<br />Longitude where the sample was taken.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>breddegrad</td>
      <td>breddegrad som prøven ble tatt på.<br />Latitude where the sample was taken.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>bunndyp</td>
      <td>bunndyp der prøven er tatt.<br />Bottomdepth where the sample is taken.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaperPrøver</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>unik identifikasjon av et objekt</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator, tildelt av dataleverendør/dataforvalter. Den lokale identifikatoren er unik innenfor navnerommet, ingen andre objekter har samme identifikator.<br />NOTE: Det er data leverendørens ansvar å sørge for at denne lokale identifikatoren er unik innenfor navnerommet.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til objektet, starter med to bokstavs kode jfr ISO 3166. Benytter understreking  ("_") dersom data produsenten ikke er assosiert med bare et land.<br />NOTE 1 : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og vil registreres i "INSPIRE external  Object Identifier Namespaces Register"<br />Eksempel: NO for Norge.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen.<br />NOTE Maksimum lengde er valgt for å tillate tidsregistrering i henhold til  ISO 8601, slik som  "2007-02-12T12:12:12+05:30" som versjonId.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>beskrivelse av kvaliteten på stedfestingen<br />Merknad: Denne er identisk med ..KVALITET i tidligere versjoner av SOSI.</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>0..1</td>
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
      <td>0..1</td>
    </tr>
    <tr>
      <td>første<wbr />Datafangstdato</td>
      <td>dato når data ble registrert/observert/målt første gang, som utgangspunkt for første digitalisering<br /><br />Merknad:<br />førsteDatafangstdato brukes hvis det er av interesse å forvalte informasjon om når en ble klar over objektet. Dette kan for eksempel gjelde datoen for første flybilde som var utgangspunkt for registrering i en database.</td>
      <td>Date<wbr />Time</td>
      <td>1</td>
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
FellesEgenskaperPrøver

#### SledePrøver

Prøver som er samlet inn med slede.<br />Samples collected by the use of sledge.

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
      <td>sted som objektet eksisterer på.<br />Location where the object exists.</td>
      <td>Punkt</td>
      <td>1</td>
    </tr>
    <tr>
      <td>redskap</td>
      <td>type redskap benyttet for prøvetakingen.<br />Name of equipment used for the sampling.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>arter<wbr />Enhet</td>
      <td>enhet for antall arter.<br />Unit used for number of species.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>biomasse<wbr />Enhet</td>
      <td>enhet benyttet for biomasse for det aktuelle redskapet.<br />Unit used for weigth for this equipment.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>individer<wbr />Enhet</td>
      <td>enhet benyttet for individer for det aktuelle redskapet.<br />Unit used for number of individuals for this equipment.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesEgenskaperPrøver</th>
    </tr>
    <tr>
      <td>referanse<wbr />Stasjon</td>
      <td>referansestasjon, unik innen MAREANO.<br />Reference number during MAREANO prosject (superstation).</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>tokt<wbr />Nummer</td>
      <td>toktnummer ved Havforskningsinstituttet.<br />Cruise number at IMR.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>arter</td>
      <td>antall forskjellige arter funnet i prøven.<br />Nos different species in the sample.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>individer</td>
      <td>individer funnet i prøven.<br />Individuals in the sample.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>biomasse<wbr />Vekt</td>
      <td>biomasse av arter funnet i prøven.<br />Weight of individuals in sample.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>lengdegrad</td>
      <td>lengdegrad som prøven ble tatt på.<br />Longitude where the sample was taken.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>breddegrad</td>
      <td>breddegrad som prøven ble tatt på.<br />Latitude where the sample was taken.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>bunndyp</td>
      <td>bunndyp der prøven er tatt.<br />Bottomdepth where the sample is taken.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaperPrøver</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>unik identifikasjon av et objekt</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator, tildelt av dataleverendør/dataforvalter. Den lokale identifikatoren er unik innenfor navnerommet, ingen andre objekter har samme identifikator.<br />NOTE: Det er data leverendørens ansvar å sørge for at denne lokale identifikatoren er unik innenfor navnerommet.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til objektet, starter med to bokstavs kode jfr ISO 3166. Benytter understreking  ("_") dersom data produsenten ikke er assosiert med bare et land.<br />NOTE 1 : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og vil registreres i "INSPIRE external  Object Identifier Namespaces Register"<br />Eksempel: NO for Norge.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen.<br />NOTE Maksimum lengde er valgt for å tillate tidsregistrering i henhold til  ISO 8601, slik som  "2007-02-12T12:12:12+05:30" som versjonId.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>beskrivelse av kvaliteten på stedfestingen<br />Merknad: Denne er identisk med ..KVALITET i tidligere versjoner av SOSI.</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>0..1</td>
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
      <td>0..1</td>
    </tr>
    <tr>
      <td>første<wbr />Datafangstdato</td>
      <td>dato når data ble registrert/observert/målt første gang, som utgangspunkt for første digitalisering<br /><br />Merknad:<br />førsteDatafangstdato brukes hvis det er av interesse å forvalte informasjon om når en ble klar over objektet. Dette kan for eksempel gjelde datoen for første flybilde som var utgangspunkt for registrering i en database.</td>
      <td>Date<wbr />Time</td>
      <td>1</td>
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
FellesEgenskaperPrøver

#### GenerelleEgenskaperPrøver (abstrakt)

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
      <td>lokal identifikator, tildelt av dataleverendør/dataforvalter. Den lokale identifikatoren er unik innenfor navnerommet, ingen andre objekter har samme identifikator.<br />NOTE: Det er data leverendørens ansvar å sørge for at denne lokale identifikatoren er unik innenfor navnerommet.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til objektet, starter med to bokstavs kode jfr ISO 3166. Benytter understreking  ("_") dersom data produsenten ikke er assosiert med bare et land.<br />NOTE 1 : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og vil registreres i "INSPIRE external  Object Identifier Namespaces Register"<br />Eksempel: NO for Norge.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen.<br />NOTE Maksimum lengde er valgt for å tillate tidsregistrering i henhold til  ISO 8601, slik som  "2007-02-12T12:12:12+05:30" som versjonId.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>beskrivelse av kvaliteten på stedfestingen<br />Merknad: Denne er identisk med ..KVALITET i tidligere versjoner av SOSI.</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>0..1</td>
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
      <td>0..1</td>
    </tr>
    <tr>
      <td>første<wbr />Datafangstdato</td>
      <td>dato når data ble registrert/observert/målt første gang, som utgangspunkt for første digitalisering<br /><br />Merknad:<br />førsteDatafangstdato brukes hvis det er av interesse å forvalte informasjon om når en ble klar over objektet. Dette kan for eksempel gjelde datoen for første flybilde som var utgangspunkt for registrering i en database.</td>
      <td>Date<wbr />Time</td>
      <td>1</td>
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
      <td><a href="https://register.geonorge.no/sosi-kodelister/generelle-konsepter/5.1/m%C3%A5lemetode">https://register.geonorge.no/sosi-kodelister/generelle-konsepter/5.1/m%C3%A5lemetode</a></td>
    </tr>
  </tbody>
</table>
