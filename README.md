# BOUZID MOUSSAAB ABDELBARIE
# El-moubarek fayçal


Question 5 ) 

     Apres la creation de la classe IObjetDessinable ,  cette interface doit etre implementée par la class TrainCercle et la class Visage
        Puis on ajoute la declaration des  2 methodes deplacer() et dessiner(Graphics g) qui sont en commun entre (class TrainCercle et ses sous class) et avec Forme Circulaire reguliere. 

Question 7 )    Lors de l’implementation de l’interface IObjetDessinable notre visage ne s’est pas afficher car la classe dessin ne dessine que les TrainsCercles

            Solution : on passe a notre classe Dessin et on modifie le type de la listeTrain par "IObjectDessinable" . le listeTrain Comportera dans ses cases le type Visage et le type TrainCercle
            ce qui nous oblige aussi a modifier le type variables de la methode  ajouterObjet(),animer(),paintComponent() situer dans la class dessin par le nom de l'interface IObjectDessinable a fin de pouvoir ajouter les 2 type Visage et TrainCercle. 

            on passe au main on modifie le type des tableau ListTrain a IObjectDessinable puis on ajoute dans la 3 eme case l'objet visage

Question 17)  Pour créer des nouveaux mouvement faut créer une classe pour chaque mouvement.
Vu que la classe AnimationForme a besoin de deux methode deplacer() et dessiner() pour ce compiler correctement et elle est liée a une interface IObjetAnimable et donc on liée l’interface IObjetAnimable avec l’interface IObjetDessinable Et On faisant une appelle au constructeur de classe IObjetAnimable on définissent le premier paramètre comme une forma étoile et le deuxième un mouvement circulaire (MvtCirculaire) dans la classe main comme suit d.ajouterObjet(new AnimationForme( new Etoile(350, 100, 50, 8.f, Color.yellow, Color.YELLOW), new MvtCirculaire(250, 250, 180, 0, 5) )); On oura une étoile animable avec des mouvements circulaires.



