# Analisi di una rete sociale di Twitter - Primo Progetto di Social Computing

## Autori Progetto

*   [Emanuele Lena](https://github.com/emanuelena49) - 142411
*   [Ilaria Fenos](https://github.com/ilariaf) - 142494
*   [Massimiliano Baldo](https://github.com/massimilianobaldo) - 142296
*   [Simone Dalla Pietà](https://github.com/Simonedp) - 141995

## Descrizione Progetto

L’obiettivo del progetto è di reperire una porzione della rete sociale del social network  Twitter, per poi fare un’analisi applicando alcune delle più tipiche tecniche di studio dei grafi. 

Nel dettaglio, si intende: 

- Reperire i dati pubblici di 5 di profili di partenza e dei profili a loro direttamente correlati (“followers” e “followings”)

- Reperire i dati di ulteriori profili casuali (scelti secondo certi criteri [inserire riferimento a sezione])

- Costruire un grafo che rappresenta la rete sociale, dove

    - i nodi sono i profili scaricati
    
    - gli archi (diretti) indicano una relazione di follower → followed (“chi segue chi”)

- Applicare le più comuni tecniche di analisi sul grafo, quali:

    - visualizzazione del grafo

    - misura delle distanze e centralità

    - calcolo della copertura minima

    - stima della “small-world-ness” del grafo

- Calcolo delle correlazioni tra le variabili calcolate

Per maggiori informazioni, consultare la relazione.

## Descrizione directory

Questa è una descrizione delle directory e dei file contenuti:

- il file "Analisi_Rete_Sociale_Twitter.ipynb" è il notebook Jupyter contenente l'intero codice;

- il file "Relazione.pdf" è il file contenente la relazione del progetto;

- la directory "analysis_data" contiene i risultati dell’analisi sul grafo, in particolare:

    - il file "graph_data.pickle" contiene i risultati delle operazioni effettuate sul grafo, sotto forma di dict python serializzata;

    - i files "df_correlation_rho.csv", "df_correlation_tau.csv" contengono le tabelle rappresentati la correlazione di Pearson Rho e la correlazione di Kendall Tau tra tutte le misure di centralità;

- la directory "data" contiene i dataset finali utilizzati per costruire il grafo; questi dataset contengono tutte le informazioni sui profili scaricati e sulle relazioni tra di essi (veder relazione e notebook per i dettagli sulla loro struttura):

    - il file "df_users.csv" contiene tutti gli utenti facenti parte del grafo con tutti i loro dati;

    - il file "df_relations.csv" contiene le relazioni tra gli utenti;

    - il file "df_accurate_relations_sample_100.csv" contiene i risultati della chiamata "show_friendship" su un campione di utenti; questo dataset non è stato utilizzato per creare il grafo;

- la directory "networkx_graphs" contenente i file riguardanti la rete sociale, in particolare:

    - il file "twitter_graph.pickle" contiene la serializzazione del grafo;

    - il file "twitter_graph_undirected" contiene la serializzazione del grafo indiretto;

    - il file "twitter_graphs_screen_names.pickle" contiene la serializzazione del grafo che usa gli screen_names degli utenti al posto degli id come nome di nodi;

- la directory "pyvis_graphs" contenente i grafi interattivi generati con la libreria pyvis; 

- la directory "raw_data" contiene i dataset generati dalle singole chiamate, questi dataset sono stati riuniti nei dataset presentati nella cartella "data".
