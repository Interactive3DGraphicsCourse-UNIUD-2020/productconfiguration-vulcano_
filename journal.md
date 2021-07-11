# 2 luglio
- Ricerca online di modelli 3D e di esempi di configuratori di prodotto. 
- Scelta del modello del cuscino e ricerca di ispirazione per i materiali. Prime idee: creare tre materiali, di cui uno che simuli la seta.

# 3 luglio
- Creazione della scena (con orbit controls e stats) e inserimento di due istanze del modello. 
- Inizio scrittura di uno shader per il materiale seta con BRDF che tiene conto della componente diffusiva e speculare della luce, usando una point light e alcune texture di cui era dotato il modello 3D. 
- Progettazione e inizio creazione della GUI per la selezione dei materiali.

![prime prove 3 luglio](imgs/screenshot_3_luglio.png)

# 5 luglio
- Modifica texture per il materiale seta.
- Idea: il secondo materiale simulerà un tessuto metallizzato. Ricerca di foto di riferimento e texture.
- Continuo dello sviluppo della GUI.

# 6 luglio
- Scrittura fragment shader per il materiale metallizzato usando inizialmente una combinazione di BRDF diffusiva e speculare e provando varie texture map. Decisione di usare la sola BRDF speculare e di variare il colore modificando il parametro cspec.
- Decisione di creare come terzo materiale la pelle. Ricerca di texture ma non ancora implementato lo shader.
- Aggiunta una terza istanza del modello e continuazione dell'implementazione della GUI.

![aggiunta terzo modello e applicazione materiale metallizzato](imgs/screenshot_6_luglio.png)

# 7 luglio
- Ricerca e aggiunta alla scena di una cubemap usata come environment map negli shader. 

![aggiunta cubemap e modifiche aspetto](imgs/screenshot_7_luglio.png)

- Prova di vari tipi di tone mapping. 
- Affinamento dell'aspetto dell'applicazione: aggiunto menù del sito con logotipo creato in Photoshop e cura dell'aspetto della GUI.

# 8 luglio
- Studio delle luci disabilitando la cubemap e utilizzando delle geometrie a sfera come aiuto: scelta di aggiungere altre due point lights e di posizionarle sia davanti sia dietro agli oggetti. 

![studio delle luci](imgs/screenshot_8_luglio.png)

- Aggiunta di un piano semistrasparente e scelta di non renderizzarvi sopra ombre. 
- Rifinitura dell'aspetto dell'interfaccia tramite aggiunta di finti breadcrumbs ed eliminazione degli stats.
- Decisione di modificare il primo materiale in modo che simuli il cotone e non la seta: usata BRDF lambertiana.

# 9 luglio
- Completamento degli shader per cotone e tessuto metallizato con l'aggiunta delle normal map. Malfunzionamenti e difficoltà a individuarne la causa, poi scoperta che three.js non riesce a creare tangenti per una geometria non indexed. Problema risolto grazie a una funzione trovata online che rende indexed una geometria che non lo è.

# 10 luglio
- Scrittura del fragment shader per il materiale pelle: BRDF con termine diffusivo e speculare.
- Prove di altre cubemap ma scelta di tenere quella corrente. Idea: nominare il set di cuscini "Sunset" per creare un legame fra prootto e ambientazione. 
- Rifinitura GUI.
- Pulizia del codice ed eliminazione dei file non utilizzati.
- Aggiunte limitazioni per gli orbit controls (evitato il pan, regolamentato lo zoom).

![scena finale con materiale pelle](imgs/scena_pelle.png)

# 11 luglio
- Modifica degli orbit controls in modo da regolamentare il movimento verticale della telecamera.
- Scrittura del file readme e del file journal (precedentemente tenuto solo in locale in semplice formato txt).

