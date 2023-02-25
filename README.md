# dicio-android-wiki-catala
Wiki no oficial de l'assistent virtual de codi obert Dicio per a Android.

## TRADUCCIÓ
### Traducció de l'aplicació
Per a traduir l'aplicació, utilitzar el portal:
https://hosted.weblate.org/projects/dicio-android/strings/

### Traducció dels skills
Els arxius de traducció són ubicats al directori del codi font de Dicio, concretament a la següent carpeta:
- ../app/src/main/sentences/<cll>
- <cll> equival als directoris amb els arxius de traducció "en|ca|etc" 
- Els arxius de traducció són en format "dslf" i utilitzen expressions regulars.

#### Vet aqui una petita descripció de la sintaxi:
- "|" separa diferents possibles paraules en una posició determinada de la frase.
- "?" especifica que l'expressió que la precedeix és opcional.
  - Ex. "paraula1|paraula2?": el "2" d'abans de "?" és opcional.
  - Ex. "(paraula1|paraula2)?": "paraula1" o "paraula2", són opcionals.
- "<>"  indica que les expressions de dins són opcionals per a la paraula o caracter que la precedeixen.
        Ex. "contrari<a?> pot ser "contrari" o contraria"
"<es|a?>" i "<a?>" són opcions alternatives que indiquen que la lletra "es" o "a" són opcionals en la paraula.
        Ex. "contrari<es|a?> pot ser "contrari", "contraries" o "contraria"
- "(quelles sont) (pour? moi)?" és una altra opció que indica que les paraules "quelles sont" i "pour moi" són opcions i poden aparèixer en qualsevol ordre. El "?" indica que "pour" és opcional.
- "les|le?" indica que "les" o "le" són opcions per a la paraula següent.
- "lletra|text" indica que la paraula pot ser "lletra" o bé "text".
- "(de (la musique|chanson)?)?" és una altra opció que indica que la paraula "de" és opcional i pot ser seguida per "la musique" o "chanson" o bé no apareixer.
