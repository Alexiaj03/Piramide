# Piramide
C#
Per spiegare come ho effettuato il compito allego parti di codice e le commento.

``` C#
public static int Piani( int mattoni )
        {
            int piani;
            int blocchi;
            int i;
```
il numero di mattoni e' dato dal programma, quindi non ce bisogno di dichiarare "mattoni", bensi andiamo a dichiarare piani, che ci senvirà per il conteggio dei piani, blocchi, che ci ritornerà quanti ne sono avanzati, e i, un indice.

``` C#
if (mattoni ==1){
                return 1;
            }
            else{
                mattoni =mattoni -1;
            }
       
```
questa è una semplice istruzione di if.

``` C#
 while (mattoni > 0){
                blocchi =blocchi +8^i;
                mattoni = mattoni -blocchi;
                piani= piani +1;
                i=i +1;
            }
            return (piani);
```
tramite un while diamo come istruzione che i mattoni devono essere maggiori di 0, dopodiche a ogni giro i blocchi utilizzati saranno uguali ai blocchi utilizzati in precedenza +8 elevati a i; i parte da 0 e si incrementa a ogni giro.
per finire ritorna il numero dei piani.
