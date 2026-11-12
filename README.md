# Bildbibliotek – appuppdateringar

Detta är den **offentliga distributionsplatsen** för Bildbibliotek för macOS.

Det privata källkodsprojektet, användarnas importerade PDF-filer, bildindex och arbetsmaterial finns **inte** här.

## Status
Ingen signerad appversion är publicerad ännu. Uppdateringsflödet `appcast.xml` skapas först när en riktig Sparkle-signaturnyckel finns och den första versionen har verifierats.

## Vad publiceras här?
- `appcast.xml`: Sparkles publika uppdateringsinformation.
- `Bildbibliotek-x.y.z.zip`: färdigbyggd app som har EdDSA-signerats och verifierats.
- Versionsanteckningar utan privata uppgifter.

**Publicera aldrig:** Swift-källkod, kunddokument, PDF-bibliotek, index.json, privata signeringsnycklar, osignerade testbyggen eller interna arbetsfiler.

## Säkerhet
Sparkle använder HTTPS samt EdDSA-signering av uppdateringsarkivet. Den privata EdDSA-nyckeln förvaras lokalt på utvecklarens Mac, inte i GitHub. Ett vanligt Apple-konto ger inte Developer ID-signering/notarisering, så ett slutligt installationstest i macOS krävs.

## Dokumentation
[Sparkle – officiell publiceringsguide](https://sparkle-project.org/documentation/publishing/)

**Detta projekt är bara för appdistribution.** För frågor om funktioner eller källkod används det separata privata projektet.
