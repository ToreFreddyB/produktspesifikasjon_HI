### Datamodell

**Kilde:** [SOSI UML XMI-fil](https://sosi.geonorge.no/svn/SOSI/SOSI%20Del%203/Havforskningsinstituttet/MareanoReferansestasjoner-20210601.xml)

<a href="mareano-referansestasjoner-uml_feature_catalogue.png" title="Klikk for stor visning"><img src="mareano-referansestasjoner-uml_feature_catalogue.png" alt="Datamodell mareano_referansestasjoner_uml" style="max-width: 100%; height: auto;" /></a>

#### GenerelleEgenskaperStasjoner (abstrakt)

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
      <td>opphav</td>
      <td>referanse til opphavsmaterialet, kildematerialet, organisasjons/publiseringskilde<br />Merknad:<br />Kan også beskrive navn på person og årsak til oppdatering</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
  </tbody>
</table>

#### Referansestasjon

Mareanostasjon hvor det er tatt bunnprøver.<br />-- Definition --<br />Mareano station where bottom samples are collected.

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
      <td>Punkt</td>
      <td>1</td>
    </tr>
    <tr>
      <td>referanse<wbr />Stasjon</td>
      <td>referansestasjon, unik innen MAREANO.<br />-- Definition --<br />Reference number during MAREANO prosject (superstation).</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>tokt<wbr />Nummer<wbr />Bunnprøver</td>
      <td>toktnummer ved Havforskningsinstituttet.<br />-- Definition --<br />Cruise number at IMR.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>tokt<wbr />Nummer<wbr />Video</td>
      <td>toktnummer ved Havforskningsinstituttet.<br />-- Definition --<br />Cruise number at IMR.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>bomtrål<wbr />Antall</td>
      <td>antall prøver som er samlet inn med bomtrål.<br />-- Definition --<br />Number of samples collected by the use of beamtrawl.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>boxcorer<wbr />Antall</td>
      <td>antall prøver som er samlet inn med boxcorer.<br />-- Definition --<br />Number of samples collected by the use of boxcorer.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>grabb<wbr />Antall</td>
      <td>antall prøver som er samlet inn med grab.<br />-- Definition --<br />Number of samples collected by the use of grab.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>slede<wbr />Antall</td>
      <td>antall prøver som er samlet inn med slede.<br />-- Definition --<br />Number of samples collected by the use of sledge.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>multicorer<wbr />Antall</td>
      <td>antall prøver som er samlet inn med multicorer (tar 6 prøver i gangen, regnes som 1 prøvetagning).<br />-- Definition --<br />Number of samples collected by the use of multicorer (six samples are taken in one operation and counts as one sample).</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>ctd<wbr />Antall</td>
      <td>antall ctd-målinger som er utført.<br />-- Definition --<br />Number of ctd measurements.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>video<wbr />Opptak<wbr />Antall</td>
      <td>antall videoopptak ved stasjonen.<br />-- Definition --<br />Number of recordings made at the station.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>bunnprøver<wbr />Antall</td>
      <td>antall bunnprøver samlet inn totalt.<br />-- Definition --<br />Number of bottom measurements collected in total.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>prøver<wbr />Totalt</td>
      <td>totalt antall prøver<br />-- Definition --<br />Total number of samples</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>stasjons<wbr />Type</td>
      <td>type stasjon: Videostasjon, Videostasjon + Bunnprøver eller Annet.<br />-- Definition --<br />type of station: Videostasjon (videostation), Videostasjon + Bunnprøver (videostation and bottom sample) or Annet (other).</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>stasjons<wbr />Type<wbr />Kode</td>
      <td>kode for type av stasjon: Type=1 = Videostasjon. Type 2 = Videostasjon + Bunnprøver. Type 3 = Annet.<br />-- Definition --<br />code for type of station: Type=1 = Videostasjon (videostation). Type 2 = Videostasjon + Bunnprøver (videostation and bottom sample). Type 3 = Annet (other).</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>lengdegrad</td>
      <td>lengdegrad som prøven ble tatt på.<br />-- Definition --<br />Longitude where the sample was taken.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>breddegrad</td>
      <td>breddegrad som prøven ble tatt på.<br />-- Definition --<br />Latitude where the sample was taken.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>bunndyp</td>
      <td>bunndyp der prøven er tatt.<br />-- Definition --<br />Bottomdepth where the sample is taken.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>lokasjon</td>
      <td>lokasjon der opptaket ble tatt.<br />-- Definition --<br />Location where the recording was made.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kommentar</td>
      <td>kommentar om opptaket<br />-- Definition --<br />Further information about the recording</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>bunnprøve<wbr />År</td>
      <td>prøvetakingsÅr.<br />-- Definition --<br />Year of sample.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>video<wbr />År</td>
      <td>opptaksÅr.<br />-- Definition --<br />Year of recording.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaperStasjoner</th>
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
      <td>opphav</td>
      <td>referanse til opphavsmaterialet, kildematerialet, organisasjons/publiseringskilde<br />Merknad:<br />Kan også beskrive navn på person og årsak til oppdatering</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
GenerelleEgenskaperStasjoner

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
