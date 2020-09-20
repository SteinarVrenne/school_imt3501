Potential Drivers
-----------------

..  a. Identify the potential external and internal drivers for the security requirements
In this section we will identify the documents that influence our security requirements.

.. According to Datatilsynet will the norwegian "personopplysningsloven" cover all requirements from the GDPR in addition to the national adjustments the GDPR allows nations to perform. This is why it is not mentioned explicitly furher down in the document.

.. https://www.datatilsynet.no/regelverk-og-verktoy/lover-og-regler/om-personopplysningsloven-og-nar-den-gjelder/ "Det betyr at alle norske regler om behandling av personopplysninger må passe inn i personvernforordningens system for å være gyldige."

Internal
--------

We will be using the agile-version of Microsoft's Secure Development Lifecycle as we assume it is required by our company to be using a framework for our development. The use of this framework will add certain requirements, some of which will be necessary to enforce every sprint while others are only once in a while or once for the entire project. 

External
--------

.. - Direktoratet for e-helse
  - Messaging standard for pregnancy termination
    - Meldingsstandard for sending av applikasjonsmeldinger angående abort.
  - ebXML-framework
    - Standard for applikasjonsmeldinger generelt i helsevesenet.
  - Applikasjonskvittering v1.1
    - Standard for svar på applikasjonsmeldinger.
.. Grunnen til at de to over er tatt med:
.. https://ehelse.no/standarder/om-standardisering-i-e-helse/referansekatalogen-for-e-helse

The Directorate of e-health have several messaging standards that the "Forskrift om IKT-standarder i helse og omsorg" enforce the use of. These are techinical standards that dictate how the system is supposed to communicate with other health systems:

* ebXML-framework - https://ehelse.no/standarder/ebxml-rammeverk-v1.1
* Applikasjonskvittering v1.1 - https://ehelse.no/standarder/applikasjonskvittering-v1.1
* Tilbakemelding om feil i mottatt melding [#]_
* Henvisning v1.1 - https://ehelse.no/standarder/henvisning-v1.1
* Mikrobiologi v1.4 [Svarrapport] - https://ehelse.no/standarder/mikrobiologi-v1.4-svarrapport
* Immunologi v1.4 [Svarrapport] - https://ehelse.no/standarder/immunologi-v1.4-svarrapport
* Medisinsk biokjemi v1.4 [Svarrapport] - https://ehelse.no/standarder/medisinsk-biokjemi-v1.4-svarrapport
* Patologi v1.4 [Svarrapport] - https://ehelse.no/standarder/patologi-v1.4-svarrapport
* Radiologi v1.4 [Svarrapport] - https://ehelse.no/standarder/radiologi-v1.4-svarrapport
* Melding om svangerskapsavbrudd (v4.1) - https://ehelse.no/standarder/melding-om-svangerskapsavbrudd-v4.1

The "Kjernejournalforskriften" has some additional requirements regarding users and how their access to the health records is to be acheived. https://lovdata.no/dokument/SF/forskrift/2013-05-31-563

The "Helseregisterloven – hregl" states in article 21 that there must be implemented systems for access control and logging. In addition the system must allow the user to view, alter and delete what the system has registered on them

Personopplysningsloven holds within it the GDPR in addition to the national adjustments the GDPR allows nations to perform. The following articles will greatly affect the development of our system:

* Article 12, 13, 14 states we have to inform the subject of the their rights in an understandable way, how they may contact us and how long and why we plan to keep their information.
* Article 15, 16, and 17 gives the subject the right to demand we give them all the information we have about them, to correct any information we hold that is currently wrong, and to demand we delete all of the data we have collected on them.
* Article 20 gives the subject the right to get access to their own data in an electronic format or to directly move their data to another data processor.
* According to article 21 and 22 the subject has the right to protest our use of the data either when used for automated decisions or in profiling for marketing.
* Article 25 states our software must by default use the most privacy friendly settings only altering them after permission is given by the subject.
* Article 32 states that if we identify a high risk need to include pseudonymization  and cryptographic securing of personal information, as well as securing the systems confidentiality, intergrity, and availability. In the case of a techinical or physical event the system should quickly be able to return to a state where the personal information can be accesessed and managed.
* Article 33 states that in the case of a breach of security for the personal information all users are to be informed whithin 72 hours. This response is to include the type of breach, the consequences, an aproximation of how many have been affected as well as the actions we plan to take to mitigate the consequences. All the informaiton mentioned is also to be documented for the future.

.. - Norske lover
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
.. - IKT-standarder - https://lovdata.no/dokument/SF/forskrift/2015-07-01-853


.. rubric:: Footnotes
.. [#] https://ehelse.no/standarder/tilbakemelding-om-feil-i-mottatt-melding
