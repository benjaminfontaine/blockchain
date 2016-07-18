#Comment est-ce que ça marche ? (Cas du bitcoin)

<!-- .slide: class="page-title" -->



## Le registre ou ledger

<figure>
    <img src="ressources/ledger-simplifie.png" alt="structure" style="float:left ; width: 50%"/>
</figure>

<figure class="fragment" data-fragment-index="1">
    <img src="ressources/ledger-distribue.png" alt="structure" style="float:left ; width: 50%"/>
</figure>

 [Source : www.imponderablethings.com](http://www.imponderablethings.com/2013/07/how-bitcoin-works-under-hood.html)



## Portefeuille ou wallet
</br>
</br>
</br>
<div style="text-align:center;font-weight:bold;">
C'est un programme permettant de générer des jeux de clés privées-publiques.
Clés qui permettront de générer des adresses pour envoyer ou reçevoir de l'argent. 
Chaque utilisateur d'une blockchain en possède un.
</div>



## Protection de l'identité : la signature électronique

</br>
La clé privée est **indispensable** pour pouvoir utiliser ses bitcoins.

<!-- .element class="fragment" data-fragment-index="1" -->
**Aucun recours en cas de perte ou de vol.**

</br>

<!-- .element class="fragment" data-fragment-index="2" -->
La clé publique est générée à partir de la clé privée. L'inverse est impossible.

</br>

<!-- .element class="fragment" data-fragment-index="3" -->
Ces clés permettent :

<!-- .element class="fragment" data-fragment-index="4" -->
- l'anonymité de l'utilisateur : la clé publique est la seule à transiter sur le réseau

<!-- .element class="fragment" data-fragment-index="5" -->
- de s'assurer que seul l'utilisateur est en droit de dépenser ses bitcoins


<div style="padding-left:30px" class="fragment" data-fragment-index="6">> Toutes les transactions sont signées numériquement avec la clé privée</div> 
  
<div style="margin:5px 0px 5px 60px;padding:5px 0px 5px 20px;border:1px solid #222222;background-color:lightgrey" class="fragment" data-fragment-index="7"> signature(clé privée, contenu transaction) = signature numérique</div>
    
<div style="padding-left:30px" class="fragment" data-fragment-index="8">> Tous les noeuds du réseau vérifie les signature numériques des transaction reçues</div>
  
<div style="margin:5px 0px 5px 60px;padding:5px 0px 5px 20px;border:1px solid #222222;background-color:lightgrey" class="fragment" data-fragment-index="9">verification(clé publique, signature, contenu transaction) = OK ou KO</div>



## Une transaction
</br>
</br>
</br>
<div style="text-align:center;font-weight:bold;">
Echange de valeur entre un ou plusieurs utilisateurs.
</div>
</br>
</br>

<!-- .element class="fragment" data-fragment-index="1" -->
Composée de : 

<!-- .element class="fragment" data-fragment-index="1" -->
- addresses expéditeurs et destinataires

<!-- .element class="fragment" data-fragment-index="1" -->
- montant

<!-- .element class="fragment" data-fragment-index="1" -->
- règles optionnelles d'execution

<!-- .element class="fragment" data-fragment-index="1" -->
- champs technique

<!-- .element class="fragment" data-fragment-index="1" -->
- crypto-signature

</br>
</br>

<!-- .element class="fragment" data-fragment-index="2" -->
Faire une transaction, c'est autoriser l'utilisateur qui possède la clé privée correspondante à l'adresse destinataire
à utiliser le montant. 



## Un block
</br>
</br>
</br>

<div style="text-align:center;font-weight:bold;">
Un mayon de la blockchain. Contient plusieurs transactions + des metadonnées
</div>

<figure>
    <img src="ressources/block-content.jpg" alt="structure" style="width: 100%"/>
</figure>



## Hashage

- hash(données arbritraires) = empreinte de taille constante (256 bits pour SHA256)

- facile à calculer et donc à vérifier

- impossible de déduire les données d'entrée à partir du hash

- imprédictible : on change un bit de données, le hash change totalement 

</br>
</br>
<!-- .element class="fragment" data-fragment-index="1" -->
SHA256('Ceci est un message que je vais hasher')


<div class="fragment" data-fragment-index="2" style="background-color:lightgrey;padding:5px 5px 5px 20px;margin-bottom:5px;">
3bafc6c7cd65c024772da01e217439cb797bca112828471824716a89c2772c76
</div>

</br>
</br>

<!-- .element class="fragment" data-fragment-index="3" -->
SHA256('Ceci est un message que je vais hasher.')


<div class="fragment" data-fragment-index="4" style="background-color:lightgrey;padding:5px 5px 5px 20px;margin-bottom:5px;">
56f89ffd4594e91617f0f2bdeb3ab0df18c49a6a53ed57f7a221319e1d1d085b
</div>



## Structure de la blockchain

<figure>
    <img src="ressources/structure-blockchain.jpg" alt="structure" style="width: 90%"/>
</figure>

<!-- .element class="fragment" data-fragment-index="1" -->
**      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;=>Très difficile de modifier un bloc surtout s'il est ancien**



## Déroulement d'une transaction

<figure class="transaction-cadre">
    <img class="transaction-img-1" src="ressources/transaction-process-step-1.jpg" alt="transaction-process"/>
</figure>



## Déroulement d'une transaction

<figure class="transaction-cadre">
    <img class="transaction-img-1" src="ressources/transaction-process-step-2-1.jpg" alt="transaction-process"/>
</figure>



## Déroulement d'une transaction

<figure class="transaction-cadre">
    <img class="transaction-img-1" src="ressources/transaction-process-step-2-2.jpg" alt="transaction-process"/>
</figure>



## Déroulement d'une transaction

<figure class="transaction-cadre">
    <img class="transaction-img-1" src="ressources/transaction-process-step-2-3.jpg" alt="transaction-process"/>
</figure>



## Déroulement d'une transaction

<figure class="transaction-cadre">
    <img class="transaction-img-1" src="ressources/transaction-process-step-2-4.jpg" alt="transaction-process"/>
</figure>



## Déroulement d'une transaction

<figure class="transaction-cadre">
    <img class="transaction-img-2" src="ressources/transaction-process-step-3-1.jpg" alt="transaction-process"/>
</figure>



## Déroulement d'une transaction
<figure class="transaction-cadre">
    <img class="transaction-img-2" src="ressources/transaction-process-step-3-2.jpg" alt="transaction-process"/>
</figure>




## Déroulement d'une transaction

<figure class="transaction-cadre">
    <img class="transaction-img-2" src="ressources/transaction-process-step-3-3.jpg" alt="transaction-process"/>
</figure>



## Déroulement d'une transaction

<figure class="transaction-cadre">
    <img class="transaction-img-2" src="ressources/transaction-process-step-3-4.jpg" alt="transaction-process"/>
</figure>



## Déroulement d'une transaction

<figure class="transaction-cadre">
    <img class="transaction-img-2" src="ressources/transaction-process-step-3-5.jpg" alt="transaction-process"/>
</figure>



## Déroulement d'une transaction

<figure class="transaction-cadre">
    <img class="transaction-img-2" src="ressources/transaction-process-step-3-6.jpg" alt="transaction-process"/>
</figure>



## Déroulement d'une transaction

<figure class="transaction-cadre">
    <img class="transaction-img-2" src="ressources/transaction-process-step-3-7.jpg" alt="transaction-process"/>
</figure>



## Déroulement d'une transaction

<figure class="transaction-cadre">
    <img class="transaction-img-2" src="ressources/transaction-process-step-3-8.jpg" alt="transaction-process"/>
</figure>



## Déroulement d'une transaction

<figure class="transaction-cadre">
    <img class="transaction-img-2" src="ressources/transaction-process-step-4.jpg" alt="transaction-process"/>
</figure>



## Déroulement d'une transaction

<figure class="transaction-cadre">
    <img class="transaction-img-2" src="ressources/transaction-process-step-5-1.jpg" alt="transaction-process"/>
</figure>



## Déroulement d'une transaction

<figure class="transaction-cadre">
    <img class="transaction-img-2" src="ressources/transaction-process-step-5-2.jpg" alt="transaction-process"/>
</figure>



## Déroulement d'une transaction

<figure class="transaction-cadre">
    <img class="transaction-img-2" src="ressources/transaction-process-step-5-3.jpg" alt="transaction-process"/>
</figure>



## Déroulement d'une transaction

<figure class="transaction-cadre">
    <img class="transaction-img-2" src="ressources/transaction-process-step-5-4.jpg" alt="transaction-process"/>
</figure>



## Déroulement d'une transaction

<figure class="transaction-cadre">
    <img class="transaction-img-2" src="ressources/transaction-process-step-6.jpg" alt="transaction-process"/>
</figure>



## Proof of work 1/2

<div  class="fragment" data-fragment-index="1" style="text-align:center;font-weight:bold;">
La clé de voute de la blockchain (jusqu'à ce qu'on trouve mieux).
</div>
</br>

<!-- .element class="fragment" data-fragment-index="2" -->
**Son but :** 

<!-- .element class="fragment" data-fragment-index="2" -->
Permettre de trouver le consensus sur le prochain block à insérer 
et faire en sorte que ce soit coûteux

<!-- .element class="fragment" data-fragment-index="3" -->
**Comment :**

<!-- .element class="fragment" data-fragment-index="3" -->
Pour insérer le prochain block de la blockchain, les mineurs hashent le block qu'ils souhaitent insérer,
et doivent croiser les doigts (très fort, 1 chances sur 10^19) pour que le hash produit remplisse les critères fixés par 
le protocole (actuellement : commençant par 17 zéros).


<figure class="fragment" data-fragment-index="4">
    <img src="ressources/aiguille.jpeg" alt="structure" style="width: 60%"/>
</figure>



## Proof of work 2/2

**Temps de résolution :**
 
Pour un ordinateur de bureau standard : 
<!-- .element class="fragment" data-fragment-index="1" -->
1 an et demi de calcul 

Pour l'ensemble des mineurs : 
<!-- .element class="fragment" data-fragment-index="2" -->
10 minutes 

</br>
<!-- .element class="fragment" data-fragment-index="3" -->
**Les plus :** 


<!-- .element class="fragment" data-fragment-index="3" -->
- établi un consensus sur les transaction valides et leur ordonnancement

<!-- .element class="fragment" data-fragment-index="3" -->
- sécurise efficacement le système car coûte du temps et de l'argent aux mineurs

</br>

<!-- .element class="fragment" data-fragment-index="4" -->
**Les moins :** 

<!-- .element class="fragment" data-fragment-index="4" -->
- Pas du tout écologique

<!-- .element class="fragment" data-fragment-index="4" -->
- limite beaucoup la vitesse de validation des transactions


</br>

<div class="fragment" data-fragment-index="5" style="text-align:center;font-weight:bold;">
Des alternatives comme la proof of stake ou la proof of burn sont actuellement considérées dans nombre de blockchains
</div>



## La double-dépense : définition

</br>
</br>
La double dépense est le fait qu'un utilisateur essaye de dépenser une monnaie 
qui a déja utilisé dans une transaction précédente.


</br>
</br>

<!-- .element class="fragment" data-fragment-index="1" -->
La blockchain prévient la majorité de ces cas en ordonnançant les transactions grâce à sa structure.

</br>
</br>

<!-- .element class="fragment" data-fragment-index="2" -->
On ne peut pas simplement rédépenser la monnaie dans une autre transaction 
car la nouvelle serait automatiquement invalidée lors de la vérification par les mineurs.

</br>
</br>

<!-- .element class="fragment" data-fragment-index="3" -->
Cependant la double dépense reste possible du fait que la blockchain n'est pas une chaîne sur un seul niveau.



## La double-dépense : Side-chain
</br>
</br>
</br>

<figure>
    <img src="ressources/sidechain.png" alt="sidechain" style="width: 100%"/>
</figure>



## La double-dépense : cas initial

<figure>
    <img src="ressources/double-depense-1.jpg" alt="sidechain" style="width: 100%"/>
</figure>



## La double-dépense : cible du fraudeur

<figure>
    <img src="ressources/double-depense-2.jpg" alt="sidechain" style="width: 100%"/>
</figure>



## La double-dépense : cible du fraudeur

<figure>
    <img src="ressources/double-depense-3.jpg" alt="sidechain" style="width: 100%"/>
</figure>

<!-- .element class="fragment" data-fragment-index="1" -->
**N'est jamais arrivé car cela nécessite que le fraudeur résolve la POW avant tout le monde plusieurs fois d'affilées.**

<!-- .element class="fragment" data-fragment-index="2" -->
**Pour cela, il lui faut posseder au moins 51% de la puissance globale du réseau blockchain.**