## Regler 
- En ekstern dynamisk liste må enten bare inneholde IP Adresser / Domeneliste eller URL liste
### URL Liste
- Ikke inkluder *HTTP* og *HTTPS når du definerer tillat eller avvis liste. 
For eksempel, skriv `www.paloaltonetworks.com` eller `paloaltonetworks.com`, ikke `https://www.paloaltonetworks.com
- Elementer i listen må være en eksakt match og gjør ikke forskjell på store og små bokstaver
- For å tillate/hindre alle webområder i paloaltonetworks.com, legg `*.paloaltonetworks.com` til listen, dette vil 
dermed gjelde underdomener også som `mail.paloaltonetworks.com`
- Dette gjelder også suffikser; hvis du vil tillate/blokkere paloaltonetworks.com/en/US, legg `paloaltonetworks.com/* til listen
- Hvis du vil ekskludere/inkludere domain suffix som paloaltonetworks.com.au, benytt `/` til slutt f.eks.: `*.paloaltonetworks.com/`
- Blokker/Tillat liste supporterer wildcard mønster Tegnene `. / ? & = ; +` anses som separatorer. Enhver substring separert med tegnene 
- Kommentarer kan starte med # eller ; 
