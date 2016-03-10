# Présentation du concept de la blockchain

<!-- .slide: class="page-title" -->



## Bitcoin et blockchain

La blockchain est la technologie sous-jacente à la crypto-monnaie Bitcoin.

Le Bitcoin a mauvaise réputation :

<figure class="fragment" data-fragment-index="1" style="display: block; float: left; margin: 30px 0; width: 50%">
    <img src="ressources/fluctuation.jpeg" alt="fluctuation" style="margin: auto;"/>
</figure>

<figure class="fragment" data-fragment-index="2"  style="display: block; float: left; margin: 30px 0; width: 50%">
    <img src="ressources/blackmail.png" alt="chantage" style="margin: auto;"/>
</figure>

<figure class="fragment" data-fragment-index="3"  style="display: block; float: left; margin: 30px 0; width: 50%">
    <img src="ressources/drogue.jpg" alt="drogue" style="margin: auto;"/>
</figure>

<figure class="fragment" data-fragment-index="4"  style="display: block; float: left; margin: 30px 0; width: 50%">
    <img src="ressources/hitmen.jpg" alt="hitmen" style="margin: auto;"/>
</figure>




## Les problèmatiques adressées par la blockchain

<figure class="fragment" data-fragment-index="1"  style="display: block; margin: auto; width: 30%">
    <img src="ressources/not_bitcoin.jpeg" alt="not-bitcoin"/>
</figure>

<!-- .element class="fragment" data-fragment-index="2" -->
Ce système vise à répondre aux problèmatiques suivantes du bitcoin :


<!-- .element class="fragment" data-fragment-index="2" -->
- Désintermédiation : Échange des informations directement entre utilisateurs 

<!-- .element class="fragment" data-fragment-index="3" -->
** => Echange peer-to-peer**

<!-- .element class="fragment" data-fragment-index="2" -->
- Traçabilité : Empêcher que l'on donne deux fois le même bitcoin

<!-- .element class="fragment" data-fragment-index="4" -->
** => Garde les traces de transaction dans un registre**

<!-- .element class="fragment" data-fragment-index="2" -->
- Consensus distribué : Garantir la monnaie sans autorité centralisée

<!-- .element class="fragment" data-fragment-index="5" -->
** => les utilisateurs conservent ce registre et vérifient les transactions**



## Qu'est-ce que la blockchain ?

- un grand livre de compte...
- distribué...
- sans organe central de contröle...
- infalsifiable...
- et qui contient un historique fiable des transactions effectuées depuis le lancement du système.



## Quelques définitions

</br>
*Registre (ledger)* : chaîne de blocks partagés par tous les noeuds


</br>
</br>
*Block* : unité de base de la blockchain, contient plusieurs transactions

</br>
</br>
*Transaction* :

- addresse expéditeur et destinataire
- data
- règles optionnelles d'execution
- champs technique
- crypto-signature



## Structure de la blockchain

<figure>
    <img src="ressources/blockchain-structure.png" alt="structure" style="width: 100%"/>
</figure>


<!-- .element class="fragment" data-fragment-index="1" -->
Chaque block se connecte avec le précedent en intégrant le hash du block précédent dans le calcul de son hash.


<!-- .element class="fragment" data-fragment-index="2" -->
**=>Très difficile de modifier un bloc surtout s'il est ancien**



## Ordonnancement des transaction

<!-- .element class="fragment" data-fragment-index="1" -->
- Les mineurs choissisent une ou plusieurs transactions en attente 
et essayent de placer un block contenant ces transactions.

<!-- .element class="fragment" data-fragment-index="2" -->
- Chaque block est identifié par son hash.
Pour placer un block, les mineurs doivent calculer ce hash.

</br>
<!-- .element class="fragment" data-fragment-index="3" -->
**Proof of work** : le hash généré par les mineurs doit correspondre à certain critères définis par le protocole
Les mineurs utilisent une donnée d'ajustement (nonce) pour essayer de générer un hash correct.

<!-- .element class="fragment" data-fragment-index="3" -->
Très dur de déterminer un hash : il faut des années de calcul à un ordinateur standard. 



## En quoi est-ce révolutionnaire ?

</br>

<div class="fragment" data-fragment-index="1" style="background-color: #EEEEEE; color: red; padding: 5px 20px; text-align:center">
  "La chaîne de blocs permet aux gens qui ne se font pas confiance de collaborer 
  sans avoir à passer par une autorité centrale neutre. Autrement dit, c’est une machine à créer de la confiance."
</div>
 
</br>
</br>

<div class="fragment" data-fragment-index="2" style="background-color: #EEEEEE; color: red; padding: 5px 20px; text-align:center">
  "La chaîne de blocs est un registre public de confiance, que tout le monde peut partager et inspecter, mais qu’aucun utilisateur unique ne contrôle."
</div>

</br>
</br>

<div class="fragment" data-fragment-index="3" style="background-color: #EEEEEE; color: red; padding: 5px 20px; text-align:center">
  "L’expansion des chaînes de blocs est redoutable pour “le marché de la confiance”, qui comprend les institutions et bureaucraties centralisées comme les banques, les chambres de compensation et les autorités gouvernementales"
</div>
