# Simulatore di Sonar e Sottomarino

Questo progetto è un simulatore di sonar creato utilizzando Python. Il simulatore permette agli utenti di utilizzare un sonar per localizzare e usare il sistema di missili guidati torpedo per eliminarli.

## Funzionalità

- **Simulazione del Sonar**: Il simulatore include un sonar, simulato in modo semi-realistico. Gli utenti possono localizzare bersagli, conoscere la loro velocità posizione e direzione.

- **Eliminazione dei bersagli**: Il simulatore include una simulazione di lancio di missili torpedo, contro i bersagli localizzati. Il sistema di guida automatica dei missili è simulato in modo realistico.

- **Interfaccia Utente Intuitiva**: L'interfaccia utente è progettata per essere intuitiva e facile da usare, consentendo agli utenti di interagire facilmente con il simulatore.

## Requisiti

- Python 3.x
- Librerie Python: [pygame](https://www.pygame.org/) [pygame-widgets](https://pygamewidgets.readthedocs.io/en/stable/)

## Installazione

1. Assicurati di avere Python 3.x installato sul tuo sistema.
2. Installa i requisiti utilizzando il seguente comando:
  
   ***pip install pygame pygame-widgets***

   
5. Clona la repository sul tuo computer o scarica la release
6. Esegui game.py (nel caso di repository) o sonar.exe (nel caso di release


## Come usare il sonar

Appena entrati nell'applicazione si avranno due schermi, uno a sinistra che occupa metà dello schermo, chiamato Sonar Display, e uno a destra più piccolo sotto il pannello di controllo, chiamato Information Display

Nella guida abbrevierò Sonar Display in SD e Information Display in ID.

I due schermi saranno all'inizio spenti, e devono essere accesi tramite le due levette, chiamate Circuit Breakers.

Una volta premuti i due Circuit Breakers, gli schermi si accenderanno.

Sul SD inizieranno ad apparire dei puntini rossi, quelli sono i segnali rilevati dal sonar e rappresentano le navi nemiche, mentre sull'ID verrà indicato che nessun segnale è selezionato.

Sul pannello di controllo sono presenti 4 pulsanti, Next, Deselect, Target, Fire.

- Next: Con questo pulsante sarà possibile selezionare una nave. Sul SD apparirà un quadrato blu che circonda il segnale selezionato, mentre sull'ID appariranno informazioni base del bersagio come direzione, velocità e coordinate, sopra alla scritta "SELECTED"
- Deselect: Con questo pulsante si può deselezionare una nave, il quadrato blu nel SD verrà rimosso e non verranno più mostrate le informazioni nell'ID
- Target: Bersaglia la nave selezionata, per fare effetto una nave deve essere selezionata tramite next precedentemente. Sulla nave selezionata apparirà un simbolo del bersaglio e nell'ID il testo selected diventerà targeted
- Fire: Dopo aver bersagliato una nave, con questo comando verrà lanciato un Torpedo, che si direzionerà in automatico verso il bersaglio e lo eliminerà.

