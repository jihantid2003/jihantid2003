
#include <stdio.h>
int main (){
 char matrix [5][5]= {
  {'1','2','3','4','5'},
  {'7','a','c','8','d'},
  {'c','9','4','z','8'},
  {'5','6','p','n','3'},
  {'2','9','t','m','k'},
 };
 int i,j;
 printf(" la matrice original :\n ");
 for(i=0;i<5;i++){
   for(j=0;j<5;j++){
    printf("%c" ,matrix[i][j]);
   }
   printf("\n");
 }
 printf("matrice avec les ligens ? indice pair :\n");
  for(i=0;i<5;i++){
   for(j=0;j<5;j++){
    printf("%c" ,matrix[i][j]);
   printf("\n");
 
}printf("matrice avec les ligens ?indice impair de chaque linge :\n");
 
  for(i=0;i<5;i++){
   for(j=0;j<5;j+=2){
    printf("%c" ,matrix[i][j]);
   }
   printf("\n");
   
 }
  return 0;
}
}



tp 
#include <stdio.h>
#include <string.h>
#include <stdlib.h>

char *ChargerChaine(int N) {
    char *chaine = (char*)malloc(N+1); 
    printf("Veuillez saisir la chaine:\n");
    fgets(chaine, N, stdin);
    chaine[strcspn(chaine, "\n")] = '\0'; 
    return chaine;
}

int Longueur(char *ch) {
    return strlen(ch);
}

void ChargerTab(char *p, char Tab[]) {
    strcpy(Tab, p);
}

void InverserTab(char Tab[], char T[], int m) {
    for (int i = 0; i < m; i++) {
        T[i] = Tab[m-i-1];
    }
}

void AfficherTab(char Tab[], int m) {
    for (int i = 0; i < m; i++) {
        printf("%c", Tab[i]);
    }
    printf("\n");
}

int main() {
    int n;
    printf("Veuillez saisir la taille maximale de la chaine:\n");
    scanf("%d", &n);
    char *ch = ChargerChaine(n);
    int m = Longueur(ch);
    char Tab[m], T[m];
    ChargerTab(ch, Tab);
    printf("La chaine originale: \n");
    AfficherTab(Tab, m);
    InverserTab(Tab, T, m);
    printf("La chaine inversée:\n");
    AfficherTab(T, m);
    free(ch);
    return 0;
}
<!---
jihantid2003/jihantid2003 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
