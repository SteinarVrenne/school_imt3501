Potential Drivers
-----------------

..  a. Identify the potential external and internal drivers for the security requirements
In this section we will identify the documents that influence our security requirements. According to Datatilsynet will the norwegian "personopplysningsloven" cover all requirements from the GDPR in addition to the national adjustments the GDPR allows nations to perform. This is why it is not mentioned explicitly furher down in the document.

.. https://www.datatilsynet.no/regelverk-og-verktoy/lover-og-regler/om-personopplysningsloven-og-nar-den-gjelder/ "Det betyr at alle norske regler om behandling av personopplysninger må passe inn i personvernforordningens system for å være gyldige."

Internal
--------




External
--------

The Directorate of e-health have several messaging standards that the "Forskrift om IKT-standarder i helse og omsorg" enforce the use of. These are the following standards:
- ebXML-framework - https://ehelse.no/standarder/ebxml-rammeverk-v1.1
- Applikasjonskvittering v1.1 - https://ehelse.no/standarder/applikasjonskvittering-v1.1
- Tilbakemelding om feil i mottatt melding - https://ehelse.no/standarder/tilbakemelding-om-feil-i-mottatt-melding
- Henvisning v1.1 - https://ehelse.no/standarder/henvisning-v1.1
- Mikrobiologi v1.4 [Svarrapport] - https://ehelse.no/standarder/mikrobiologi-v1.4-svarrapport
- Immunologi v1.4 [Svarrapport] - https://ehelse.no/standarder/immunologi-v1.4-svarrapport
- Medisinsk biokjemi v1.4 [Svarrapport] - https://ehelse.no/standarder/medisinsk-biokjemi-v1.4-svarrapport
- Patologi v1.4 [Svarrapport] - https://ehelse.no/standarder/patologi-v1.4-svarrapport
- Radiologi v1.4 [Svarrapport] - https://ehelse.no/standarder/radiologi-v1.4-svarrapport
- Melding om svangerskapsavbrudd (v4.1) - https://ehelse.no/standarder/melding-om-svangerskapsavbrudd-v4.1

The "Kjernejournalforskriften" has some additional requirements regarding users and how their access to the health records is to be acheived. https://lovdata.no/dokument/SF/forskrift/2013-05-31-563

The "Helseregisterloven – hregl" states in article 21 that there must be implemented systems for access control and logging. In addition the system must allow the user to view, alter and delete what the system has registered on them

- Direktoratet for e-helse
  - Messaging standard for pregnancy termination
    - Meldingsstandard for sending av applikasjonsmeldinger angående abort.
  - ebXML-framework
    - Standard for applikasjonsmeldinger generelt i helsevesenet.
  - Applikasjonskvittering v1.1
    - Standard for svar på applikasjonsmeldinger.
.. Grunnen til at de to over er tatt med:
.. https://ehelse.no/standarder/om-standardisering-i-e-helse/referansekatalogen-for-e-helse
- Norske lover
  .. - Kjernejournalforskriften
    - https://lovdata.no/dokument/SF/forskrift/2013-05-31-563
    - §9 sier systemet vårt må sørge for at tilgang gis til en entydig identifiserbar person i et viss tidsrom.
  .. - Forskrift om IKT-standarder i helse og omsorg
    - https://lovdata.no/dokument/SF/forskrift/2015-07-01-853
    - §5 sier man skal følge de to første kravene fra e-helse direktoratet.
    - §6 beskriver hvilke regler som må følges for forskjellige typer meldinger.
  .. - Helseregisterloven – hregl
    - https://lovdata.no/dokument/NL/lov/2014-06-20-43#KAPITTEL_1
    - Artikkel 21
      - Tilgangsstyring, logging
      - kryptering av personlig identifiserbar informasjon
    - Artikkel 24
      - Rett til innsyn
    - Artikkel 25
      - Rett til sletting
  - Personopplysningsloven
    - https://lovdata.no/dokument/NL/lov/2018-06-15-38/#KAPITTEL_gdpr-3-1
    - Applikasjonen må la brukeren untytte sine rettigheter
      - Retting, sletting, innsyn, fratrekkelse fra AI bestemmelser,
    - Artikkel 25
      - Personvern som standard
    - Artikkel 32.
      - pseudonymisering og kryptering av personopplysninger
      - Forsvar av CIA
    - Artikkel 33.
      - Melding om brudd og dokumentasjon av tidligere brudd.







.. - E-helse direktoratet - https://ehelse.no/standarder/om-standardisering-i-e-helse/referansekatalogen-for-e-helse#Informasjonssikkerhet
  - link til liste - https://ehelse.no/standarder

  - Lov om helseregistre - https://lovdata.no/dokument/NL/lov/2014-06-20-43
  - IKT-standarder - https://lovdata.no/dokument/SF/forskrift/2015-07-01-853
