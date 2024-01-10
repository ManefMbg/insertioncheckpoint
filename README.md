1-  Function Declaration:

PROCEDURE insertion_sort(var tab : ARRAY_OF INTEGER;)

2- Initialize Variables:

VAR
    i, j, n, temp: INTEGER;
BEGIN

3- Get Array Length:

    n:= tab.length;
    
4- Outer Loop (i):    
    FOR i FROM 1 TO n-1 DO

5- Store Current Element and Initialize Inner Loop (j):    
        temp:=tab[i];
        j:=i-1;
        
6- Inner Loop (while):        
        WHILE (j>=0) and (tab[j]>temp) DO
            tab[j+1]:=tab[j];
            j:=j-1
        END_WHILE
        
7- Place Current Element in Correct Position:    

              tab[j+1]:=temp;
    END_FOR
END
