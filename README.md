# Mise en place de l'API
Tableau json d'articles aleatoires
### Documentation
my-json-server.typicode est un faux server REST en ligne
### Demarer le fake server 
         my-json-server.typicode.com/nom_utilisateur_github/repository/

Dans le cas du server des articles ce sera:

_my-json-server.typicode.com/light-int/blog/article_

        {
        "id":1,
        "nom":"MENDE",
        "prenom":"Dimitri",
        "desc":"Coach de la cohorte des developpeur Web",
        "img":"https://lacastafiore.github.io/ecole241/okacode/images/Kakashi.jpg",
        "link":"#"
       },
	     {
        "id":2,
        "nom":"OBAME NZOGHO",
        "prenom":"Billy Marc Paul",
        "desc":"Tout ce qui est beau m'attire, j'aime donc la creativite, le travail, le code, et surtout la vie",
        "img":"https://lacastafiore.github.io/ecole241/okacode/images/Billy.jpg",
        "link":"https://light-int.github.io/ecole241/profil/index.html"
	     }
       
Et pour avoir un seul profil

_my-json-server.typicode.com/light-int/blog/article/1_

        {
        "id":1,
        "nom":"MENDE",
        "prenom":"Dimitri",
        "desc":"Coach de la cohorte des developpeur Web",
        "img":"https://lacastafiore.github.io/ecole241/okacode/images/Kakashi.jpg",
        "link":"#"
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
