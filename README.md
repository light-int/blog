# Mise en place de l'API
Tableau json d'articles aleatoires
### Documentation
my-json-server.typicode est un faux server REST en ligne
### Demarer le fake server 
         my-json-server.typicode.com/nom_utilisateur_github/repository/

Dans le cas du server des articles ce sera:

_my-json-server.typicode.com/light-int/blog/article_

		{
		"id": 1,
		"titre": "Des bijoux fantaisie de créateurs à découvrir !",
		"description": "Alors qu’il y a quelques années de cela l’appellation de bijoux \"fantaisie\" renvoyait 			principalement à des bijoux bon marché de basse qualité, ce n’est plus du tout le cas aujourd’hui. La preuve, il 		n’y a qu’à voir les créateurs qui sont présents sur la boutique multimarques de Mademoiselle Sissi. Cette dernière 		dévoile des bijoux dont les créateurs rivalisent d’imagination et d’esthétisme dans leur approche de style autour 		des bijoux.\\r\\nLes gemmes comme le Lapis lazuli et la Labradorite sont travaillées très finement et apportent 		ainsi une touche d’élégance à chaque modèle de bague. Quant à leur design, comme tout bijou ethnique qui se 			respecte, ils sont surtout inspirés de pays, de civilisations et de peuples lointains, d’où leur originalité et 		leur intemporalité. Sans oublier que pour limiter au maximum les risques d’allergie, l’argent utilisé par la 			créatrice est essentiellement du 925 Sterling, que l’on appelle communément aussi de \"l’argent massif\".			\\r\\nLes inconditionnels de ce métal précieux vous confirmeront sans doute que le poinçon 925 n’est ni plus ni 		moins que le gage de la pureté de l’argent. Plus précisément, les bijoux sont composés à 92,5 % d’argent. Sinon, 		les 7,5 % restants sont les métaux indispensables utilisés dans l’alliage. En effet, exceptionnellement mou, 			l’agent ne peut être rigidifié qu’en l’associant avec du zinc ou du cuivre.",
		"date": "26/03/2018",
		"categorie": "Style",
		"auteur": "BRIXTON DOE",
		"image": "https://www.blogbijoux.info/images/articles/bijoux-104438.jpg",
		"commentaires": [
		{
		  "message": "Lorsqu’on est passionné ou collectionneur invétéré de bijoux, on est en perpétuelle recherche de la plus belle pièce. On multiplie alors les lieux et les canaux d’achat. Essayez ces trois là !",
		  "nom": "Alicia",
		  "date": "25/04/2017"
		}
		]
		},
		{
		"id": 2,
		"titre": "Ma première collection de chaussures",
		"description": "J’ai pensé à mes chaussures préférées, des Miu Miu achetées à Cannes pour le festival, les plus chères que j’ai jamais eues. Elles sont en PVC transparent avec une fleur sur le dessus, de vrais escarpins de cendrillon. Si je les aime autant c’est parce que leur transparence allonge la jambe et qu’elles se marient avec tout. Aussi, début 2018 commençait la tendance PVC sur les défilées, ça tombait bien. Du coup j’ai décidé de partir d’une paire de chaussures toute transparente et d’utiliser mes pieds comme une page blanche. Dessus j’ai peint, j’ai colorié, j’ai collé les petites formes colorées de mon identité visuelles. Les formes sont en suédine sur les escarpins et en cuir vernis sur les bottines (inspiration 60S, Courrèges, Carel… mes marques préférées).\\r\\nStress intense lorsqu’il a fallu présenter tout ça devant l’équipe Sarenza au complet, et par chance ils ont tous adoré! Ensuite j’ai travaillé avec leur styliste Julien Martinez pour les dessins techniques et le lancement des premiers prototypes. On en a fait 2 en tout, le second pour modifier le positionnement des formes, et puis c’était bon ! Il a fallu attendre Juillet pour recevoir les premières chaussures dans ma pointure et shooter la campagne de communication. On a fait ça dans mon studio, avec un équipe que j’ai pu choisir : Sasha Marro comme photographe et Sacha Giraudeau pour la maquillage. Le duo de choc avec qui j’avais travaillé pour les visuels de la Palette Primaire. Les filles du studio m’ont aidée pour trouver le stylisme et faire le set design et on a passé une journée très gaie (vidéo backstages ici).\\r\\nVoilà ! Les chaussures sont en vente sur le site de Sarenza depuis ce matin et j’ai un peu la boule au ventre ! J’espère qu’elles vont plaire et se vendre. La pire hantise se serait qu’elles se retrouvent soldées en Janvier, non?",
		"date": "02/01/2018",
		"categorie": "mode",
		"auteur": "BRIXTON DOE",
		"image": "https://www.elsamuse.com/wp-content/uploads/2018/11/SHOES_5_SHOT_1786-def1-rvb.jpeg",
		"commentaires": [
		{
		  "message": "j'adore cette collection",
		  "nom": "Annie Jeffy",
		  "date": "05/02/2018"
		},
		{
		  "message": "Tres belles ses chaussures",
		  "nom": "Laurent",
		  "date": "10/02/2018"
		}
		]
		}
       
Et pour avoir un seul profil

_my-json-server.typicode.com/light-int/blog/article/1_


		{
		"id": 1,
		"titre": "Des bijoux fantaisie de créateurs à découvrir !",
		"description": "Alors qu’il y a quelques années de cela l’appellation de bijoux \"fantaisie\" renvoyait 			principalement à des bijoux bon marché de basse qualité, ce n’est plus du tout le cas aujourd’hui. La preuve, il 		n’y a qu’à voir les créateurs qui sont présents sur la boutique multimarques de Mademoiselle Sissi. Cette dernière 		dévoile des bijoux dont les créateurs rivalisent d’imagination et d’esthétisme dans leur approche de style autour 		des bijoux.\\r\\nLes gemmes comme le Lapis lazuli et la Labradorite sont travaillées très finement et apportent 		ainsi une touche d’élégance à chaque modèle de bague. Quant à leur design, comme tout bijou ethnique qui se 			respecte, ils sont surtout inspirés de pays, de civilisations et de peuples lointains, d’où leur originalité et 		leur intemporalité. Sans oublier que pour limiter au maximum les risques d’allergie, l’argent utilisé par la 			créatrice est essentiellement du 925 Sterling, que l’on appelle communément aussi de \"l’argent massif\".			\\r\\nLes inconditionnels de ce métal précieux vous confirmeront sans doute que le poinçon 925 n’est ni plus ni 		moins que le gage de la pureté de l’argent. Plus précisément, les bijoux sont composés à 92,5 % d’argent. Sinon, 		les 7,5 % restants sont les métaux indispensables utilisés dans l’alliage. En effet, exceptionnellement mou, 			l’agent ne peut être rigidifié qu’en l’associant avec du zinc ou du cuivre.",
		"date": "26/03/2018",
		"categorie": "Style",
		"auteur": "BRIXTON DOE",
		"image": "https://www.blogbijoux.info/images/articles/bijoux-104438.jpg",
		"commentaires": [
		{
		  "message": "Lorsqu’on est passionné ou collectionneur invétéré de bijoux, on est en perpétuelle recherche de la plus belle pièce. On multiplie alors les lieux et les canaux d’achat. Essayez ces trois là !",
		  "nom": "Alicia",
		  "date": "25/04/2017"
		}
		]
		} 
### Iteration 
 #### Es6
 

    // Fetch articles
    fetch('https://my-json-server.typicode.com/light-int/blog/article')
      .then(response => {
        if (response.ok) {
          return Promise.resolve(response);
        }
        else {
          return Promise.reject(new Error("Une erreur c'est produite")); 
        }
      })
      .then(response => response.json())
      .then(data => {

        data.forEach(function(item,index){
        let donnee = `
        <article class="mb-50">
            <a class="btn btn-tiny" href="#">${item.categorie}</a>
            <h2 class="med-title">${item.titre}</h2>
            <p class="tiny-text">${item.date}</p>
            <img src="${item.image}" alt="${item.titre}" class="img-responsive mb-3">
            <p class="foo">${item.description}</p>
            <a href="articles.html?id=${item.id}" class="btn btn-block">LIRE LA SUITE</a>
        </article> `;
        $('#all').append(donnee);
        })
      })
      .catch(function(error) {
        console.log(`Error: ${error.message}`);
      });


 Voir la [demo](https://my-json-server.typicode.com/light-int/hackaton-DB/user)
