# 2 luglio
- Ricerca online di esempi di configuratori di prodotto e di modelli 3D. 
- Scelta del modello del cuscino e ricerca di ispirazione per i materiali.

# 3 luglio
- Creazione della scena (con orbit controls e stats) e inserimento di due istanze del modello. 
- Inizio scrittura dello shader per il materiale cotone usando una point light, la diffuse map e la ao map scaricate insieme al modello. 
- Progettazione e inizio creazione della GUI per la selezione dei materiali.

![prime prove 3 luglio] (imgs/screenshot_3_luglio.png)

# 5 luglio
- Scelta di usare texture diverse per il materiale cotone e ricerca di texture per il tessuto metallizzato. 
- Decisione di aggiungere come terzo materiale la pelle. 
- Continuo dello sviluppo della GUI.

# 6 luglio
- Scrittura fragment shader per il materiale metallizzato usando una combinazione di BRDF diffusiva e speculare e provando varie texture map. Decisione di usare la sola BRDF speculare e di variare il colore modificando il parametro cspec.
- Aggiunta una terza istanza del modello e continuazione dell'implementazione della gui.

# 7 luglio
- Ricerca e aggiunta alla scena di una cubemap. 
- Prova di vari tipi di tone mapping. 
- Affinamento dell'aspetto dell'applicazione: aggiunto menù del sito con logotipo creato in Photoshop e cura dell'aspetto della GUI.

# 8 luglio
- Studio delle luci disabilitando la cubemap e utilizzando delle geometrie a sfera come aiuto: scelta di aggiungerne altre due e di posizionarle sia davanti sia dietro agli oggetti. Aggiunta di un piano semistrasparente e scelta di non renderizzarvi sopra ombre. 
- Rifinitura dell'aspetto dell'interfaccia tramite aggiunta di finti breadcrumbs ed eliminazione degli stats.

# 9 luglio
- Completamento degli shader per cotone e tessuto metallizato con l'aggiunta delle normal map. Malfunzionamenti e difficoltà a individuarne la causa, poi scoperta che three.js non riesce a creare tangenti per una geometria non indexed. Problema risolto grazie a una funzione trovata online che rende indexed una geometria che non lo è.

# 10 luglio
- Aggiunta del fragment shader per il materiale pelle.
- Prove di altre cubemap ma scelta di tenere questa. Idea: nominare il set di cuscini "Sunset" per creare un legame fra prootto e ambientazione. 
- Rifinitura GUI.
- Pulizia del codice ed eliminazione dei file non utilizzati.
- Aggiunte limitazioni per gli orbit controls (evitato il pan, regolamentato lo zoom).

# 11 luglio
- Modifica degli orbit controls in modo da regolamentare il movimento verticale della telecamera.
- Scrittura del file readme e del file journal (precedentemente tenuto solo in locale in semplice formato txt).

