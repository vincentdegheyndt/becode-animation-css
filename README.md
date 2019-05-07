Drill:
    Pas de difficulté particulière mis-à-part le contrôle du hover pour le troisième bouton.
    Le hover ne se faisait que via un très petite zone qui, se déplaçant justement via le hover, ne restait jamais bien longtemps sous la souris. De faite, le bouton se réinitialisait de façon assez anarchique.

    La solution fut trouvée en mettant le bouton (button3) au sein d'une div (class="area"). c'est le hover de la souris sur cette div fixe qui déclenche le déplacement du button3 via :
    
    &:hover .button3 (transform: translateX(...px))

Menu:
    Même problème de hover instable. 
    C'est lors de cette exercice que j'ai fini par trouver la solution "&:hover .qqch {...}" qui m'a permis d'activer le déplacement de l'élément mobile via un hover sur un élément fixe.
    
    Au départ, cette solution créait un déplacement entier de la colonne et pas uniquement du tiroir associé à l'icône sur lequel le hover a lieu.
    Ce problème fût réglé via le HTML en mettant les chaque élément "tiroir" au sein du li contenant l'icône respectif.

animecard:
    Quelques problèmes de z-index par rapport à la photo, la date et le texte défilant.
    Egalement des problèmes de débordement du texte et dela photo lors du hover. Rapidement réglés via un overflow hidden.
