# ATELIER-3
Se fameliariser avec les classes

#include <iostream>

using namespace std;

class Voiture{
    private :
   string marque ;        // la marque de la voiture.
 string modele  ;      // le modèle de la voiture.
 int annee    ;               // l'année de fabrication de la voiture.
 float kilometrage ;         // le kilométrage actuel de la voiture.
 float vitesse     ;        // la vitesse actuelle de la voiture.

  public :
   Voiture( marque(""), modele(""), annee(0), kilometrage(0.0), vitesse(0.0) ){

    }
     Voiture(string marque,string modele , int annee, float kilometrage ,float vitesse){
          marque ="Volkswagen" ;
    modele="Golf"   ;
    annee =  2020         ;
    kilometrage= 1000    ;
    vitesse = 120        ;

    }
    void accelerer(float valeur) {
        float valeur ;
        vitesse += valeur  ;
             }
   void  freiner(float valeur) {
      float valeur ;
      if (vitesse>0) {
      vitesse -= valeur ;}
      else vitesse = 0   }

    void   afficherInfo(){
          cout<<"voici les informations de la voiture :" <<endl ;
          cout<<" la marque de cette voiture est "<<marque<<endl ;
          cout<<" le modele de cette voiture est "<<modele<<endl ;
          cout<<" l annee de cette voiture est "<<annee<<endl ;
          cout<<" le Kilometrage de cette voiture est "<< Kilometrage<<"km"<<endl ;
          cout<<" la vitesse de cette voiture est "<<vitesse<<"km/m"<<endl ;
          }
       void   avancer(float distance) {float distance ;
                   kilometrage += distance;
                     }
  ~Voiture() {
        std::cout << "La voiture " << marque << " " << modele << " est détruite"<<endl ;
    }

}
