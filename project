#include<stdio.h>
#include<conio.h>
#include<string.h>
#include<stdlib.h>
extern void hut()

{
	system("color FC");
    static int totalCost;
    int i,j,choice,c=1,a[9],cost[9];
    for(i=0;i<9;i++) a[i]=0;
    char str[100];
    char items[9][100]={"MARGHERITA PIZZA", "DOUBLE CHEESE MARGHERITA PIZZA", "FARM HOUSE", "CHICKEN TIKKA", "NON VEG SUPREME", "CHICKEN SAUSAGE", "GREEN TEA", "WHITE TEA", "COFFEE" };
    
	printf("\nPlease Enter Customer Name\n");
    gets(str);
    printf("\nHello %s, Welcome to our Online pizza hut shop.\n",str);
    do
    {
    {
    printf("Enter\n1 - VEG PIZZA\n2 - NON VEG PIZZA\nAny other number to exit\n");
    scanf("%d",&choice);
    switch(choice) 
    {
    case 1: 
    {
    int PIZZA;
    printf("Enter\n1 - MARGHERITA PIZZA - Rs.195\n2 - DOUBLE CHEESE MARGHERITA PIZZA - Rs.295\n3 - FARM HOUSE - Rs.365\nAny other number to exit\n");
    scanf("%d",&PIZZA);
    cost[0]=195;
    cost[1]=295;
    cost[2]=395;
    switch(PIZZA) 
    {
    case 1: 
    {
    int num;
    printf("You chose MARGHERITA PIZZA - Rs.195.Are you sure to buy.If 'Yes' Enter 1 else any number\n");
    scanf("%d",&num);
    if(num==1) 
    {
    totalCost+=195;
    }
    printf("Your Cost in Cart is %d\n",totalCost);
    break;
    }
    case 2: 
    {
    int num;
    printf("You chose  DOUBLE CHEESE MARGHERITA PIZZA - Rs.295.Are you sure to buy.If 'Yes' Enter 1 else any number\n");
    scanf("%d",&num);
    if(num==1) 
    {
    a[1]++;
    totalCost+=295;
    }
    printf("Your Cost in Cart is %d\n",totalCost);
    break;

    }
    case 3: 
    {
    int num;
    printf("You chose FARM HOUSE - Rs.365.Are you sure to buy.If 'Yes' Enter 1 else any number\n");
    scanf("%d",&num);
    if(num==1) 
    {
    a[2]++;
    totalCost+=395;
    }
    printf("Your Cost in Cart is %d\n",totalCost);
    break;
    }
    default:
    {
    printf("Exit from VEG PIZZA\n");
    break;
    }
    }
    break;
	}
    case 2: 
    {
    int NON_VEG_PIZZA;
    printf("Enter\n1 - CHICKEN TIKKA - Rs.355\n2 - NON-VEG SUPREME- Rs.350\n3 - CHICKEN SAUSAGE - Rs.500\nAny other number to exit\n");
    scanf("%d",&NON_VEG_PIZZA);
    cost[3]=355;
    cost[4]=350;
    cost[5]=500;
    switch(NON_VEG_PIZZA) 
    {
    case 1: 
    {
    int num;
    printf("You chose CHICKEN TIKKA - Rs.355.Are you sure to buy.If 'Yes' Enter 1 else any number\n");
    scanf("%d",&num);
    if(num==1) 
    {
    a[3]++;
    totalCost+=355;
    }
    printf("Your Cost in Cart is %d\n",totalCost);
    break;

    }
    case 2: 
    {
    int num;
    printf("You chose NON-VEG SUPREME- Rs.350.Are you sure to buy.If 'Yes' Enter 1 else any number\n");
    scanf("%d",&num);
    if(num==1) 
    {
    a[4]++;
    totalCost+=350;

    }
    printf("Your Cost in Cart is %d\n",totalCost);
    break;
    }
    case 3: 
    {
    int num;
    printf("You chose CHICKEN SAUSAGE - Rs.500.Are you sure to buy.If 'Yes' Enter 1 else any number\n");
    scanf("%d",&num);
    if(num==1) 
    {
    a[5]++;
    totalCost+=500;
    }
    printf("Your Cost in Cart is %d\n",totalCost);
    break;
    }
    default:
    {
    printf("Exit from NON_VEG_PIZZA\n");
    break;
    }
    }
    break;
    }
    default: 
    {
    printf("Enter Valid Categories Choice\n");
    break;
    }
    }
    //printf("\n%s's cart\n",str);
    printf("\nId\tItems\t\t\tQuantity\t\t\tCost\n");
    for(i=0;i<9;i++) 
    {
    if(a[i]!=0) 
    {
    printf("\n%d\t%s\t\t%d\t\t\t\t%d\n",i,items[i],a[i],(cost[i]*a[i]));
    }
    }
    printf("\nTotal Cost :: %d\n",totalCost);
    printf("\nIf you wish to buy anything more Enter\n1 to Add Item\n2 to Delete Items \nAny other number to Exit\n");
    scanf("%d",&c);
    }
    if(c==2) 
    {
    int id;
    printf("Enter id to delete item\n");
    scanf("%d",&id);
    if(id<9&&id>0)
    {
    totalCost=totalCost-(cost[id]*a[id]);
    a[id]=0;
    }
    else
    {
    printf("Enter Valid id\n");
    }
    printf("Revised Items \n");
    printf("Id\tItems\t\t\tQuantity\t\tCost\n");
    for(i=0;i<9;i++) 
    {
    if(a[i]!=0) 
    {
    printf("%d\t%s\t\t%d\t\t%d\n",i,items[i],a[i],(cost[i]*a[i]));
    }
    }
    printf("\nTotal Cost\t\t\t\t\t%d\n",totalCost);
    printf("If you wish to buy anything more Enter\n1 to Add Item\n2 to Delete Items \nAny other number to Exit\n");
    scanf("%d",&c);
    }
    }
    while(c==1 || c==2);
    printf("\nYour Final Cost is %d\n",totalCost);
    printf("\nThanks %s for Choosing Us and Visit us again.\n",str);

}
