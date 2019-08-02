#include<stdio.h>
#include<conio.h>
#include<string.h>
#include"cse project.cpp"
#include<stdlib.h>
struct login
  {
   char uname[20];
   char pwd[20];
  }l,l1,l2;

 main()
   {
    
    system("COLOR CB");
    char c;
    do
	{
	
    int ch,found=0;
    printf("\n                                                         |******************************|");
    printf("\t\t\t\t\t\t\t\t\t\t\t | Welcome to Tip-Top Pizza hut |");
    printf("\n                                                         |******************************|");
    
    
    FILE *f=fopen("E:\\gur.txt","a+");
    printf("\n1) Create Account");
    printf("\n2) LOGIN\n");
    printf("\nEnter your choice  ");

    scanf("%d",&ch);
    if(ch==1)
    {
       printf("Enter User Name");
       fflush(stdin);
       gets(l.uname);
       printf("Enter User Password");
       fflush(stdin);
       gets(l.pwd);
       fwrite((char *)&l,sizeof(l),1,f);
       printf("Registered Successfully\n");
    }
    if(ch==2)
    {
	printf("Enter User Name");
	fflush(stdin);
	gets(l1.uname);
	printf("Enter User Password");
	fflush(stdin);
	gets(l1.pwd);
	rewind(f);
	while(fread((char *)&l2,sizeof(l2),1,f))
    {
	    if((strcmp(l2.uname,l1.uname)==0)&&(strcmp(l2.pwd,l1.pwd)==0))
        {
	    printf("\n________________________________________________________ --  LOGIN SUCCESSFULLY  -- __________________________________________________________\n            ");
	    printf("\n");
     	hut();
	    found=1;
        }
    }
	    if(found==0)
	    printf("\n");
	    printf("ERROR :: Not an authorised user\n");
	    printf("********************************");
	}
    else
    {
    printf("\nERROR :: Invalid input\n ");
    fclose(f);
	}
	
    printf("\n Do you want to continue (y/n)");
 //  c=getch(); or
 fflush(stdin);
    scanf("%c",&c);
    }
    while(c=='y'||c=='Y');
    //getch();
   }

