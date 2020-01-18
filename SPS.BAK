#include<time.h>
#include<stdio.h>
#include<conio.h>
#include<graphics.h>
#include<stdlib.h>
#include<dos.h>

void main()
{  //auto detection
   int gdriver = DETECT, gmode,ans;

   //initialize graphics mode
   initgraph(&gdriver,&gmode, "C:\\Turboc3\\BGI");

do
{

   int sum1=0, sum2=0,i,ch1,ch2;
   char name1[10], name2[10];
   clrscr();

      //details of player1
       printf("\nEnter player1 name : ");
       scanf("%s", name1);

       //details of player2
       printf("\nEnter player2 name : ");
       scanf("%s", name2);

       printf("\n");

	  textcolor(RED);

	  cprintf("GAME STARTS\n");
	     delay(2000);

	   for(i=0;i<6;i++)
	   {

	      printf("\nSelect a tool for your game\n");
	      printf("\n1.Stone\n2.Paper\n3.Scissor\n");

	      printf("\n%s's turn : ", name1);
	      scanf("%d", &ch1);
	      printf("\n%s's turn : ", name2);
	      scanf("%d", &ch2);

	    //if both select same number
	    if(ch1==ch2)
	    {
		   textcolor(MAGENTA);
	       cprintf("\n\t score of %s is %d\n",name1, sum1);
	       cprintf("score of %s is %d\n",name2, sum2);
		textcolor(BROWN);
	      cprintf("\nREDO THE MATCH\n");
		     delay(1000);
		printf("\nSelect a tool for your game\n");
		      printf("\n1.Stone\n2.Paper\n3.Scissor\n");


	      printf("\n%s's turn : ", name1);
	      scanf("%d", &ch1);
	      printf("\n%s's turn : ", name2);
	      scanf("%d", &ch2);
	    }
	   //stone<paper
	   else if(ch1==1&& ch2==2)
	    {
	       sum2+=1;
		textcolor(MAGENTA);
	       cprintf("\n\t score of %s is %d\n",name1, sum1);
	       cprintf("score of %s is %d\n",name2, sum2);

	    }
	    //stone>scissor
	    else if(ch1==1&& ch2==3)
	    {
		sum1+=1;
		 textcolor(MAGENTA);
	       cprintf("\n\t score of %s is %d\n",name1, sum1);
	       cprintf("score of %s is %d\n",name2, sum2);

	    }
	    //paper>stone
	    else if(ch1==2&&ch2==1)
	    {
		sum1+=1;
		 textcolor(MAGENTA);
		cprintf("\n\t score of %s is %d\n",name1, sum1);
		cprintf("score of %s is %d\n",name2, sum2);

	    }
	    //paper<scissor
	    else if(ch1==2&&ch2==3)
	    {
	      sum2+=1;
	       textcolor(MAGENTA);
	       cprintf("\n\t score of %s is %d\n",name1, sum1);
	       cprintf("score of %s is %d\n",name2, sum2);
	      }
	    //scissor<stone
	    else if(ch1==3&&ch2==1)
	    {
	       sum2+=1;
		textcolor(MAGENTA);
	       cprintf("\n\t score of %s is %d\n",name1, sum1);
	       cprintf("score of %s is %d\n",name2, sum2);

	    }
	    //scissor>paper
	    else if(ch1==3&&ch2==2)
	    {
	       sum1+=1;
	       textcolor(MAGENTA);
	       cprintf("\n\t score of %s is %d\n",name1, sum1);
	       cprintf("score of %s is %d\n",name2, sum2);

	    }

     }
		 if(sum1==sum2)
		 {
		      textcolor(GREEN);
		   cprintf("\nMATCH TIE\n");
		 }
		 else if(sum1>sum2)
		 {

		     textcolor(BLUE);
		   cprintf("\n%s WON!!!\n", name1);
		 }
		 else
		 {
		     textcolor(YELLOW);
		   cprintf("\n%s WON!!!\n", name2);
		 }

		 printf("\nDo you want to play again\n");

		 printf("Your response :  %s", ans);
		  scanf("%s",&ans);
     }while(ans=='y');

getch();
closegraph();
}