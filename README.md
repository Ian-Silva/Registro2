# Registro2
#include <stdio.h>
int main(void){
    struct{
    int hh;
    int mm;
    int ss;
    }HI,HO,HU;
    int ti, to, fu;

    scanf("%d:%d:%d",&HI.hh,&HI.mm, &HI.ss);
     scanf("%d:%d:%d",&HO.hh,&HO.mm, &HO.ss);



    ti = HI.hh*3600 + HI.mm*60 + HI.ss;
    to = HO.hh*3600 + HO.mm*60 + HO.ss;
    fu = ti - to;
    if(fu<0)
    fu*=-1;

    HU.hh = fu/3600;
    HU.mm = (fu%3600)/60;
    HU.ss = (fu%3600)%60;

    printf("%02d:%02d:%02d\n", HU.hh, HU.mm, HU.ss);

return 0;
}
