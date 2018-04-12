# radiocittaperta - bash script per l'ascolto in streaming di radiocittaperta★it - _La radio libera ed indipendente_

Ho creato questo script per necessità e per diletto. La necessità di accedere allo streaming di radiocittaperta.it dal mio computer in modo semplice. Il diletto nel cimentarmi nella scrittura dello stesso.

Questo script non fa altro che utilizzare software già installato, o eventualmente da installere, per ascoltare lo streaming (flusso audio dalla rete) di www.radiocittaperta.it. Non installa automaticamente il software di cui ha bisogno, si limita a farti presente che ciò di cui ha bisogno è installato o meno. In generale tutto il software di cui necessita è disponibile nei repository uffuciali di quasi tutte le distribuzioni, fatta eccezione per Red Hat e derivate.

Lo script si occupa quindi di aprire l'URL dello streaming con un PLAYER per ascoltare la radio, mantendendo il PLAYER in questione in background, senza finestra o icona nella barra.

È sufficente quindi lanciare radiocittaperta [OPZIONE] per ascoltare la radio, per interrompere l'ascolto basta lanciare nuovamente lo script. Volendo lo si può inserire nel menù delle applicazioni, creandogli un lanciatore apposito.

I PLAYER selezionati sono stati scelti in base ad un criterio di integrazione con i vari DE (KDE, GNOME, XFCE, LXDE, UNITY, ecc ecc) e funzionalità disponibili (es. la capacità di interpretare correttamente i metadati contenuti in un flusso streaming).

Per una migliore esperienza consiglio di utilizzare [Dragonplayer](https://www.kde.org/applications/multimedia/dragonplayer/) su KDE e [mpv](https://mpv.io/) sui restanti DE.

N.B Io uso [Debian](https://www.kde.org/applications/multimedia/dragonplayer/) Stretch, con KDE 5.8.6. Non ho avuto modo di provare con versioni precedenti.

Dragonplayer su KDE visualizza correttamente i metadati presenti nel flusso mp3, inserendo il titolo della canzone attualmente in onda in un menù con il simbolo "Play" nella barra delle notifiche.

Per tutti gli altri DE ho scelto di usare mpv e notify-send per mostrare le informazioni sui brani in onda, ad ogni aggiornamento quindi, compare un popup sul desktop che mostra il titolo della canzone. È possibile usare mpv anche su KDE se lo si preferisce. Utilizzare Dragonplayer con gli altri DE di contro non ha alcun senso, in quanto non si integrerebbe allo stesso modo con la barra delle notifiche.

Ho scelto di non visualizzare le informazioni sui brani in onda quando si è su terminale, dato che la comparsa improvvisa delle informazioni potrebbero creare confusione.

Dei PLAYER che ho provato Mpv e Dragonplayer sono gli unici software a mostrare le meta informazioni presenti nel flusso mp3. Tuttavia, oltre ad mpv e Dragonplayer, lo script può funzionare con altri PLAYER, inseriti in una lista, dispnibile lancianto _radiocittaperta -h_. In talune circostanze si potrebbe apprezzare il fatto che, per esempio, [mpg123](https://mpg123.de/) sia più "leggero" degli stessi dragonplayer e mpv.

Buon ascolto!

Many Thanks to Greg Wooledge, Pierre Gaston and the whole help-bash@gnu.org list 
for the support.
