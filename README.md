# ml-embarque_transpiler_c

L'objectif de ce mini-projet est de generer du code C en python permettant de faire des prediction sur un modele simple de regression lineaire.

Tout le code se trouve dans le notebook *transpiler_un_model_en_c.ipynb* 

Il suffit d'appeler la fonction `generate_file(*nom_du_modele*)' pour generer le code C correspondant dans un fichier 'code.c'

Cette fonction renverra la ligne de commande a executer dans un terminal pour compiler ce fichier 

Enfin il faut appeler l'executable genere par la commande precedente avec les donnees sur lesquels la prediction est souhaitee (1 prediction a la fois):

Par exemple:

Si l'executable s'appelle -prediction-:
        
            ./prediction 1 2 3
            
    Sera equivalant au code python model.predict([[1, 2, 3]])
