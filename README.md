#include <LedMatrixObject.h>
LedMatrixObject *led = new LedMatrixObject(2, 3, 4, 5, 6, 7, 8, 9);

unsigned char  S[16][16]{
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
};
    
unsigned char M[16][16] = {
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1},
    {1, 1, 0, 0, 0, 1, 1, 1, 1, 1, 1, 0, 0, 0, 1, 1},
    {1, 1, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 1, 1},
    {1, 1, 0, 0, 1, 0, 0, 1, 1, 0, 0, 1, 0, 0, 1, 1},
    {1, 1, 0, 0, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 0, 0, 1, 1, 1, 0, 0, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
};
unsigned char  A[16][16] = {
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 0, 0, 1, 1, 0, 0, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 0, 0, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1},
    {1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1},
    {1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
};
char K[16][16] = {
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1},
    {1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
};
char E[16][16] = {
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
  
};
char  R[16][16] = {
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1},
    {1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
};

int i;
int j;
int k;
void setup(){

}

void loop(){
  
for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[i][15] = M[i][j] ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[i][k-1] = S[i][k];

}}
}


for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[i][15] = A[i][j] ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[i][k-1] = S[i][k];

}
}
}
 
for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[i][15] = K[i][j] ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[i][k-1] = S[i][k];

}}
}
 
for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[i][15] = E[i][j] ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[i][k-1] = S[i][k];

}}
}
  
for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[i][15] = R[i][j] ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[i][k-1] = S[i][k];

}}
}
 
for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[i][15] = M[i][j] ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[i][k-1] = S[i][k];

}}
}
 
for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[i][15] = E[i][j] ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[i][k-1] = S[i][k];

}}
}
for(j=5;j<=11;j++)

{ for(i=2;i<=3;i++)
  {E[i][j] = 1;
}
for(i=7;i<=8;i++)
{E[i][j] = 1;
}
}
 
for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[i][15] = E[i][j] ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[i][k-1] = S[i][k];

}}
}
 for(j=5;j<=11;j++)

{ for(i=2;i<=3;i++)
  {E[i][j] = 0;
}
for(i=7;i<=8;i++)
{E[i][j] = 0;
}
} 
for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[i][15] = A[i][j] ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[i][k-1] = S[i][k];

}}
}
for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[i][j] = 1 ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[i][k-1] = S[i][k];

}}
}
for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[i][15] = 1 ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[i][k-1] = S[i][k];

}}
} 
for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[15][i] = M[j][i] ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[k-1][i] = S[k][i];

}}
} 
for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[15][i] = A[j][i] ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[k-1][i] = S[k][i];

}}
} 
for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[15][i] = K[j][i] ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[k-1][i] = S[k][i];

}}
} 
for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[15][i] = E[j][i] ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[k-1][i] = S[k][i];

}}
} 
for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[15][i] = R[j][i] ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[k-1][i] = S[k][i];

}}
} 
for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[15][i] = M[j][i] ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[k-1][i] = S[k][i];

}}
} 
for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[15][i] = E[j][i] ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[k-1][i] = S[k][i];

}}
}
 
for(j=5;j<=11;j++)

{ for(i=2;i<=3;i++)
  {E[i][j] = 1;
}
for(i=7;i<=8;i++)
{E[i][j] = 1;
}
}
  
for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[15][i] = E[j][i] ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[k-1][i] = S[k][i];

}}
}
 for(j=5;j<=11;j++)

{ for(i=2;i<=3;i++)
  {E[i][j] = 0;
}
for(i=7;i<=8;i++)
{E[i][j] = 0;
}
}

for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[15][i] = A[j][i] ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[k-1][i] = S[k][i];

}}
}

for(j=0;j<=15;j++)
{for(i=0;i<=15;i++)
{
  S[15][i] = 1 ;
}
for(i=0;i<=5;i++)
{
  led->setScene(S) ;
  
  led->draw();
}

for(k=1;k<=15;k++)
{for(i=0;i<=15;i++)
{
S[k-1][i] = S[k][i];

}}
}
}

