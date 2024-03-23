#include <stdio.h>
char konverto_nota (int nota) {
switch (nota / 10) {
case 10:
case 9:
return 'A'; 
case 8:
return 'B';
case 7:
return 'C';
case 6:
return 'D';
default:
return 'F';
}
}
int main () {
int nota ;
printf ("Jepni noten nga 0-100: ");
scanf ("%d" , &nota);
char shkronja = konverto_nota(nota);
printf("Nota e dhene me shkronje:%c\n", shkronja);
return 0;
}
