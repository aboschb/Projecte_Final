<b> Títol del Projecte: Les opinions dels viatgers: Anàlisi d'interaccions de Rodalies de Catalunya a X/Twitter mitjançant NLP </b>

<b> Descripció: </b>

Aquest estudi analitza la percepció i satisfacció dels usuaris de Rodalies de Catalunya a través de les interaccions en Twitter, revelant insights sobre la dinàmica comunicativa entre l'empresa i els seus usuaris. Utilitzant una combinació d'anàlisi de dades numèriques i revisió manual del contingut, juntament amb models de processament de llenguatge natural (NLP) adaptats a les limitacions lingüístiques del català, s'identifiquen les principals àrees de queixa i satisfacció. Les troballes destaquen la importància de la puntualitat, la comunicació eficaç d'incidències i la transparència com a factors crítics en la percepció del servei. Malgrat els reptes en l'aplicació de NLP, l'ús de traduccions i models preentrenats facilita l'identificació de temes emergents i el llenguatge ofensiu o sarcàstic. L'estudi conclou amb recomanacions específiques per millorar l'atenció al client i l'estratègia de comunicació de Rodalies de Catalunya, amb l'objectiu d'augmentar la satisfacció dels usuaris i millorar la percepció pública del servei.

<hr style="border-top: 1px dotted #8c8b8b;">

This study analyzes the perception and satisfaction of Rodalies de Catalunya's users through interactions on Twitter, revealing insights into the communicative dynamics between the company and its users. Utilizing a combination of numerical data analysis and manual content review, along with natural language processing (NLP) models adapted to the linguistic limitations of Catalan, the main areas of complaint and satisfaction are identified. The findings highlight the importance of punctuality, effective incident communication, and transparency as critical factors in service perception. Despite the challenges in applying NLP, the use of translations and pre-trained models facilitates the identification of emerging themes and offensive or sarcastic language. The study concludes with specific recommendations to improve customer service and the communication strategy of Rodalies de Catalunya, with the goal of increasing user satisfaction and improving the public perception of the service.

<b> Datasets: </b> Veure df_inicial i df_processat adjunts en aquest repositori

<b> Font de les dades: </b> https://twitter.com/rodalies

<b> Descripció dels datasets: </b>

- df_inicial inclou el conjunt de dades obtingudes mitjançant scraping (API de Twitter Developer).
  
- df_processat és el dataset amb noves columnes generades del preprocessament, neteja i aplicació de models. En aquest dataframe les noves columnes generades són les següents: <br>
  
• text_netejat: text sense URLs, mencions ni símbols de hashtags. <br>
• text_sense_noms: text sense noms de persona. <br>
• noms_eliminats: llista de noms eliminats. <br>
• tematica: classificació temàtica mitjançant assignació manual. <br>
• text_sense_stopwords: text sense stopwords, només dels tweets en català. <br>
• text_lemmatized: text lematitzats dels tweets en català, es mostren com a llistes de lemes. Per als tweets en castellà i anglès s'han lematitzat també (el text no apareix en forma de llista de lemes). No els tindrem en compte perquè aquesta no era la intenció, ja que el model aplicat és pel català i apareixen nombrosos errors. <br>
• classification_results: etiqueta (label) i puntuació (score) de la classificació temàtica mitjançant LDA, només pels tweets en català. <br>
• predicted_label: etiqueta de la classificació temàtica mitjançant LDA, només pels tweets en català. <br>
• confidence_score: puntuació de la classificació temàtica mitjançant LDA, només pels tweets en català. 





