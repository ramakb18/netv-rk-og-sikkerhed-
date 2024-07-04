# netv-rk-og-sikkerhed-
h1 dokumentation 
netværk:
faget netværk og sikkerhed er et felt inden for IT, der fokuserer på at designe, implementere og administrere sikre netværk. Det omfatter både teoretiske og praktiske aspekter af netværksteknologier og sikkerhedspraksis. Emner, der ofte dækkes, inkluderer:

1. Netværksgrundlæggende: Forståelse af netværksarkitekturer, protokoller (som TCP/IP), netværksmodeller (OSI-modellen), routing og switching.

2. Netværkssikkerhed: Implementering af sikkerhedsforanstaltninger som firewalls, intrusion detection/prevention systems (IDS/IPS), VPN'er, og anvendelse af krypteringsteknikker.


3. Adgangskontrol: Anvendelse af autentificerings- og autorisationsmekanismer, som brug af adgangskoder, biometrisk identifikation, og rollebaseret adgangskontrol (RBAC).

4. Sikkerhedspolitikker og procedurer: Udvikling og implementering af sikkerhedspolitikker, standarder og procedurer for at beskytte netværket og sikre overholdelse af lovgivningsmæssige krav.


Windows Server 2012 er en serveroperativsystem udgivet af Microsoft og er en del af Windows Server-familien, indeholder mange nye funktioner og forbedringer i forhold til sine forgængere. Her er nogle af de væsentlige aspekter og funktioner ved Windows Server 2012:

1. Brugergrænseflade
Windows Server 2012 introducerede en ny Metro-baseret brugergrænseflade (nu kaldet Modern UI), som også blev brugt i Windows 8. Denne brugergrænseflade er designet til at være mere touch-venlig, selvom den også fungerer med traditionelle mus- og tastaturinput.

2. Server Core Installation
Windows Server 2012 fortsatte med at tilbyde Server Core-installation, som er en minimal installationsmulighed uden grafisk brugergrænseflade. Dette hjælper med at reducere vedligeholdelses- og angrebsfladerne, hvilket kan forbedre sikkerheden og reducere ressourceforbruget.

3. Hyper-V
Windows Server 2012 kom med en stærkt forbedret version af Hyper-V, som er Microsofts virtualiseringsplatform.
 Nogle af forbedringerne inkluderer:
Support for flere virtuelle processorer og mere hukommelse pr. virtuel maskine.
Hyper-V Replica, som tillader replikering af virtuelle maskiner til en anden server for disaster recovery.

4. Storage Spaces
Introduktion af Storage Spaces, som giver mulighed for at kombinere forskellige fysiske diske i en enkelt logisk enhed. Dette gør det nemmere at administrere lagerplads og forbedrer fejltolerance.

5. Resilient File System (ReFS)
Windows Server 2012 introducerede ReFS, et nyt filsystem designet til at maksimere datasikkerhed og tilgængelighed. ReFS er designet til at håndtere store mængder data og for at minimere risikoen for korruption.

6. Dynamic Access Control
Dynamic Access Control (DAC) tillader administratorer at lave detaljerede sikkerhedspolitikker, der styrer adgangen til filer baseret på flere faktorer, såsom brugerens identitet, dataens følsomhed, og netværksforhold.

7. IP Address Management (IPAM)
Windows Server 2012 introducerede IPAM, som er et værktøj til administration af IP-adresser i netværket. IPAM giver mulighed for at overvåge, administrere og konfigurere IP-adresser og tilknyttede tjenester som DHCP og DNS.

8. Remote Desktop Services
Forbedringer i Remote Desktop Services (RDS), som inkluderer en bedre brugeroplevelse, nye muligheder for session-virtualisering og VDI (Virtual Desktop Infrastructure), samt bedre administration og implementeringsværktøjer.

9. PowerShell 3.0
Windows Server 2012 leveres med PowerShell 3.0, som tilbyder flere cmdlets og forbedringer til scripting og automatisering af administrationstasks. PowerShell Desired State Configuration (DSC) blev også introduceret, hvilket giver mulighed for deklarativ konfiguration af systemer.

10. Server Manager
Den nye Server Manager gør det muligt at administrere flere servere fra en enkelt konsol, hvilket gør det lettere at implementere og administrere serverroller og funktioner på tværs af et netværk.

Udgaver af Windows Server 2012:
Windows Server 2012 blev udgivet i fire forskellige udgaver:
Datacenter: Designet til store virksomheder med behov for omfattende virtualisering.
Standard: Designet til mindre virksomheder eller afdelinger, som ikke har store virtualiseringsbehov.
Essentials: Designet til små virksomheder med op til 25 brugere og 50 enheder.
Foundation: Designet til meget små virksomheder med op til 15 brugere.

Virtuel maskine oprettelse via hyper v proces:
•	Ind på hyper v under handling skal man vælge ”ny” og så ”virtuel maskine”
•	Hvorefter man skal gennemgå indholdet efter sit eget ønske eller krav af en opgave man har fået.
•	Man skal vælge en placering for den nye VM man er i gang med at oprette og man kan vælge standard placering eller selv vælge hvor det skal gemmes ind på sin enhed. 
•	Man skal vælge generation på den ny maskine man er i gang med at oprette, hvor der to generation 1 0g 2. 
(Forskellen er at generation 1 VM understøtter de fleste gæsteoperative system, hvor generation 2 VM under støtter de fleste 64-bit versioner af Windows og mere aktuelle versioner af Linux og FreeBSD operative system.)
•	Under processen skal man også vælge et Startup Memory, som minimum kan man starte med 2024MB og vælge Dynamic Memory.

(Hukommelse deles mellem en Hyper-V-vært og den virtuelle maskine, der kører på værten. Antallet af virtuelle maskiner, der kan køre på en enkelt vært, afhænger delvist af tilgængelig hukommelse. En virtuel maskine kan også konfigureres til at bruge Dynamic Memory. Når den er aktiveret, genvinder dynamisk hukommelse ubrugt hukommelse fra den kørende virtuelle maskine. Dette gør det muligt for flere virtuelle maskiner at køre på værten.)
•	Næste trin man skal vælge en virtuel switch til den virtuel maskine man har oprettede og angiv en størrelse. Hyper v har tre forskellige type virtuel switch som bl.a. er eksterne, interne og private.
 Forskellen på alle tre er at den eksterne VS er knyttet til et fysisk kort fra hyper v og giver adgang til netværk. 

Den interne VS isolerer de virtuelle maskiner, men tillader netværksskift mellem hyper v og de virtuelle maskiner.

Og til sidst den private VS isolerer netværk fuldstendig fra virtuelle maskiner


