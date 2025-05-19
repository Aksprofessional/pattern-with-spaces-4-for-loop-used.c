# pattern-with-spaces-4-for-loop-used.c
// c program to print pattern with spaces      A        A AB      BA ABC    CBA ABCD  DCBA ABCDEEDCBA 
// c program to print pattern with spaces
    
A        A
AB      BA
ABC    CBA
ABCD  DCBA
ABCDEEDCBA

#include <stdio.h>
int main() { 
    int i,j;
    for(i=0;i<5;i++)
    {
        for(j=0;j<=i;j++)
         printf("%c",65+j);
        for(j=0;j<=3-i;j++)
         printf(" ");
        for(j=0;j<=3-i;j++)
         printf(" ");
        for(j=i;j>=0;j--)
         printf("%c",65+j);
        printf("\n");
    }
    return 0;
}
