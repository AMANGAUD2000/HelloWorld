#include<stdio.h>
int main()
{
 int m,n,i,j,k,a[100][100];
 printf("enter the order : ");
 scanf("%d",&m);
 printf("enter elements");
 for(i=0;i<m;i++)
 {
     for(j=0;j<m;j++)
     {
         scanf("%d",&a[i][j]);

     }
 }

 i=0;
     for(j=0;j<m;j++)
     {

         printf("%d ",a[i][j]);
     }
i=i+1;
j=m-1;
     while(j==m-1&&i<m)
     {
         printf("%d ",a[i][j]);
         i=i+1;
     }
for(j=m-1;j>=0;j--)
     {

         printf("%d ",a[i][j]);
     }
     while(j==0&&i!=m-1&&i!=0)
     {
         printf("%d ",a[i][j]);
         i=i-1;
     }

     while(i==1)
     {
      for(j=0;j<m-1;j++)
      {
        printf("%d ",a[i][j]);
      }
     }




}
