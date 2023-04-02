### Structure du smart contract



##### fonction ajouter_un_heritier

Elle prend en argument l'adresse tezos tz1 d'un héritier, le pourcentage de part du wallet que veut léguer le légataire et ainsi que la durée pour laquelle le légataire peut refuser un claim.
Elle va ajouter dans une map les trois arguemnts.



##### fonction claim

C'est un entry point qui peut être appelé par la personne qui va hériter, cet entry point ne nécessite que l'adresse de la personne dont elle va hériter.
Elle va vérifier que la personne qui appelle le contrat est bien un hériter du légataire et va lancer un compteur qui sera la différence d'un timestamp et d'un autre timestamp



##### fonction refuser_un_claim

Elle prend en argument l'adresse de l'héritier dont on veut refuser le claim (en supposant qu'il ait claim avant).
Elle va vérifier que l'héritier a bien claim et ainsi changer un booléen pour dire que cet héritier n'a pas claim.
