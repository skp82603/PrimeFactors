#include<stdio.h>

int foo(int n);

int fox(int q);

int main()

{

  int n;

  printf("enter a number:");

  scanf("%d",&n);



  printf("the prime factore are \n");

  foo(n);

  return 0;



}



int foo(int n)

{

  int q;

  for(q=1;q<n;q++)

  {

    if(n%q==0)

    {

      fox(q);

    }

  }

}

int fox(int q)

{

  int i, factor,multi=1;

  for(i=1;i<q;i++)

  { if(q%i==0)

    {

     factor = i;

     multi=multi*factor;

      

    }

    

  }

  if(multi==1)

   printf("%d \t",q);

}
