# EX 7 : THREE DIMENSIONAL TRANSFORMATIONS
NAME: SRINITHI MUTHUKUMAR REG NO: 212224240161
## AIM :
 
 To implement the various transformations on three dimensional odjects using a c coding.

## EQUIPMENT REQUIRED:

●	Hardware: Personal Computer (PC)

●	Software: C Compiler

## ALGORITHM :


   Step 1 : Start.

   Step 2 : Draw an image with default parameters.

   Step 3 : Get the choice from user.

   Step 4 : Get the parameters for transformation.

   Step 5 : Perform the transformation.

   Step 6 : Display the output.

   Step 7 : Stop.

## Program :
```
#include<stdio.h>

#include<conio.h>

#include<graphics.h>

#include<math.h>

int maxx,maxy,midx,midy;

void axis()

{ getch();

cleardevice();

line(midx,0,midx,maxy);

line(0,midy,maxx,midy);

}

void main()

{
int gd,gm,x,y,z,o,x1,x2,y1,y2;

detectgraph(&gd,&gm);

initgraph(&gd,&gm," ");

setfillstyle(0,getmaxcolor());

maxx=getmaxx();

maxy=getmaxy();

midx=maxx/2;

midy=maxy/2;

axis();

bar3d(midx+50,midy-100,midx+60,midy-90,5,1);

printf("Enter Translation Factor");

scanf("%d%d%d",&x,&y,&z);

axis();

printf("after translation");

bar3d(midx+(x+50),midy-(y+100),midx+x+60,midy-(y+90),5,1);

axis();

bar3d(midx+50,midy+100,midx+60,midy-90,5,1);

printf("Enter Scaling Factor");

scanf("%d%d%d",&x,&y,&z);

axis();

printf("After Scaling");

bar3d(midx+(x50),midy-(y100),midx+(x60),midy-(y90),5*z,1);

axis();

bar3d(midx+50,midy-100,midx+60,midy-90,5,1);

printf("Enter Rotating Angle");

scanf("%d",&o);

x1=50cos(o3.14/180)-100sin(o3.14/180);

y1=50cos(o3.14/180)+100sin(o3.14/180);

x2=60sin(o3.14/180)-90cos(o3.14/180);

y2=60sin(o3.14/180)+90cos(o3.14/180);

axis();

printf("After Rotation about Z Axis");

bar3d(midx+x1,midy-y1,midx+x2,midy-y2,5,1);

axis();

printf("After Rotation about X Axis");

bar3d(midx+50,midy-x1,midx+60,midy-x2,5,1);

axis();

printf("After Rotation about Y Axis");

bar3d(midx+x1,midy-100,midx+x2,midy-90,5,1);

getch();

closegraph();
}
```
## Output :
![image](https://github.com/user-attachments/assets/3409d4aa-fcb0-4372-9637-1c47dccdbcb6)

![image](https://github.com/user-attachments/assets/fd3f19b7-ba52-4065-b337-4631e50902b3)

![image](https://github.com/user-attachments/assets/b619c3ed-4fd7-4090-8acc-1a2f1ad85861)

![image](https://github.com/user-attachments/assets/6f3abb84-63a7-402d-a44b-f10bda4f42b7)

![image](https://github.com/user-attachments/assets/ab8f5643-3fa6-4ff1-b97f-74a183db01ec)

![image](https://github.com/user-attachments/assets/e0425640-c8f0-42d1-88c6-521960d8cca1)

![image](https://github.com/user-attachments/assets/34f1d712-2cae-4daf-86e3-240759c7ccd5)

![image](https://github.com/user-attachments/assets/bd11ed95-b644-4340-bd8b-d015e857ccc6)


## Result :
Thus, the C program for performing three-dimensional transformations — including translation, scaling, and rotation about the X, Y, and Z axes — was successfully implemented and the output was verified through graphical representation.
