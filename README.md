
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
<!---
jihantid2003/jihantid2003 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
