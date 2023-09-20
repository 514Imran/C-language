#include<stdio.h>
int main()
{
    int a[3][3],b[3][3],c[3][3],i,j,k;
    printf("Enter 9 element for first matrix:");
    for(i=0; i<3; i++)
    {for(j=0; j<3; j++)
    {scanf("%5d",&a[i][j]);}}
     printf("Enter 9 element for second matrix:");
    for(i=0; i<3; i++)
    {for(j=0; j<3; j++)
    {scanf("%5d",&b[i][j]);}}
    for(i=0; i<3; i++)
    {for(j=0; j<3; j++)
    {c[i][j]=0;
    for(k=0; k<3; k++)
    {c[i][j]+=a[i][k]*b[k][j];}}}
    printf("\n Here your first matrix\n");
    for(i=0; i<3; i++)
    {for(j=0; j<3; j++)
    {printf("%5d",a[i][j]);}
     printf("\n");}
    printf("\n Here your second matrix\n");
    for(i=0; i<3; i++)
    {for(j=0; j<3; j++)
    {printf("%5d",b[i][j]);}
     printf("\n");}
    printf("\n Here multiply of both matrix\n");
    for(i=0; i<3; i++)
    {for(j=0; j<3; j++)
    {printf("%5d",c[i][j]);}
    printf("\n");}
    return 0;
}