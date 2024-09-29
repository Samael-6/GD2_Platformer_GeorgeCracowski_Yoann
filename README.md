# GD2_Platformer_GeorgeCracowski_Yoann
# 
# |||||||||||||||||||
# * BLUEPRINTS : BP *
# |||||||||||||||||||
# 
#   BP_Key :
#     Augmenter un seconde inventaire
#     Met à jour la valeur Is_Open dans le gameinstance pour pouvoir ouvrir la porte

#   BP_Door :
#        Reste fermer si BP_Key n'a pas été "récupéré"
#        Affiche ce que le joueur peut faire quand il colle la porte
# 
#   BP_HiddenSecret :
#        Change de material et de message
# 
#    BP_ChangeLevel :
#        Switch de Level entre celui de base et le level2
# 
#    BP_Joueur :
#        Gère le widget des scores
#        Intéragit avec les collectible et les objets interactifs
#        Vérifie si les objets sont toujours en contact et si ils sont iteractifs
#        Lance les interactions
# 
# |||||||||||||||||||
# * BLUEPRINTS : BC *
# |||||||||||||||||||
# 
#   BPC_CollectComponent :
#       Il permet en l'ajoutant à un acteur de collecter les autres acteurs avec les BPC_Collectible
# 
#   BPC_Collectible :
#       Il permet en l'ajoutant à un acteur il peut se faire récupérer en s'autodétruisant et agrémentant le score
# 
#   BPC_Interact :
#       Il permet d'afficher un widget avec un texte indicatif qui change selon les différents actors
# 
# ||||||||||||||||||||
# * BLUEPRINTS : BPI *
# ||||||||||||||||||||
# 
#   BPI_Interact :
#       Permet à tous les acteurs qui possède le BPI de pouvoir être interactif
# 
# ||||||||||||||||||||
# * BLUEPRINTS : BPW *
# ||||||||||||||||||||
# 
#   BPW_Interact :
#       Permet d'afficher les différents message d'intéraction
# 
#   BPW_MainMenu :
#       Permet d'afficher les différents scores
# 
# |||||||||||||||||||||||
# * BLUEPRINTS : Autres *
# |||||||||||||||||||||||
#  
#   BP_GameInstance :
#       Stock les données qui doivent perssisté d'un niveau à l'autre qui sont :
#           . Le nombre de clé
#           . La possibilité d'ouvrir la porte
#           . Le score
#  
#   BP_GameMode :
#       Je l'ai pas utilisé n'ayant pas eu recours aux données privates, n'ayant donc pas besoin de médiateur entre le GameInstance et les autres actors
# 
#  
# ||||||||||||||||||||
# *      Level       *
# ||||||||||||||||||||
# 
#   Level2 :
#       Il contient la porte vérouillé qui nécessite de la clé avec une expérience de jump initiatique.
# 
#   ThirdPersonMap :
#       Il contient la clé qui permet d'ouvrir la porte avec un parcours de pièces.
