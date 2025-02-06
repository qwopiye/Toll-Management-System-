#include<stdio.h>
#include<conio.h>

int mc=0,cj=0,mp=0,b31=0,b32=0,trc5=0,trc58=0,trc11=0, ax3=0,tra1=0,tra2=0,totalVehicles=0;
int ArrTotalVehicles[100];

int choise, vehicle, date[100], month, year;
float total=0;
float ArrTotal[100];
int first = 0;

void Add_day(){

float motor_cycle = 50.00;
float low_weight_vehiclesCJ = 550.00;
float low_weight_vehiclesMP = 600.00;
float mini_bus31 = 750.00;
float mini_bus32 = 1000.00;
float small_truckLT5T = 1000.00;
float midium_truck58 = 1250.00;
float midium_truck11 = 1600.00;
float truck3AXEL =  2000.00;
float trailer1 = 3000.00;
float trailer2 = 4000.00;


if(totalVehicles != 0){
    totalVehicles = 0;
    mc=0;
    cj=0;
    mp=0,b31=0;
    b32=0;
    trc5=0;
    trc58=0;
    trc11=0;
    ax3=0;
    tra1=0;
    tra2=0;
}


for(int i = first; i<(first+1); i++){
   printf("Please enter the full date\n");
   printf("Date: ");
      scanf("%d",&date[i]);
   printf("Month: ");
      scanf("%d",&month);
   printf("Year: ");
      scanf("%d",&year);

    printf("\n\t\t\t\tTake inputs of %d-%d-%d\n",date[i],month,year);
    printf("\t...........................\n");

    printf("\t1-motorcycle\n");
    printf("\t2-low weight vehicles(car/jeep)\n");
    printf("\t3-low weight vehicles(micro/pickup)(lower than 1.5 ton)\n");
    printf("\t4-mini bus(31 seat or less)\n");
    printf("\t5-big bus(32 srat or more)\n");
    printf("\t6-small truck(less than 5 ton)\n");
    printf("\t7-medium teruck(5-8 ton)\n");
    printf("\t8-medium truck(8-11 ton)\n");
    printf("\t9-truck(3 axel)\n");
    printf("\t10-trailer(less than 4 axel)\n");
    printf("\t11-trailer(more than 4 axel)\n\n");
    printf("\t...........................");

do
{    printf("\nPlease enter the right vehicle number and you can stop taking inputs by pressing 0: ");
    scanf("%d",&vehicle);



    switch(vehicle)
    {
    case 0:
        {
            printf("\t\t..............................\n");
            printf("\t\t\t End of %d-%d-%d\n",date[i],month,year);
            printf("\t\t..............................\n");
        }
       break;
    case 1:
        {
          mc=mc+1;
          total=total+ motor_cycle;
          printf("\t\t motorcycle, Toll added!\n");
        }
        break;

         case 2:
        {
          cj=cj+1;
          total=total+ low_weight_vehiclesCJ;
            printf("\t\t low weight vehicles(car/jeep) , Toll added!\n");
        }
        break;

         case 3:
        {
          mp=mp+1;
          total=total+ low_weight_vehiclesMP;
            printf("\t\t low weight vehicles(micro/pickup)(lower than 1.5 ton), Toll added!\n");
        }
        break;

         case 4:
        {
           b31=b31+1;
          total=total+ mini_bus31;
            printf("\t\t mini bus(31 seat or less), Toll added!\n");
        }
        break;

         case 5:
        {
          b32=b32+1;
          total=total+ mini_bus32;
          ArrTotal[i] = ArrTotal[i] + mini_bus32;
            printf("\t\t big bus(32 seat or more), Toll added!\n");
        }
        break;

         case 6:
        {
          trc5=trc5+1;
          total=total+ small_truckLT5T;
            printf("\t\t small truck(less than 5 ton), Toll added!\n");
        }
        break;

         case 7:
        {
          trc58=trc58+1;
          total=total+ midium_truck58;
            printf("\t\t medium truck(5-8 ton), Toll added!\n");
        }
        break;

         case 8:
        {
          trc11=trc11+1;
          total=total+ midium_truck11;
            printf("\t\t medium truck(8-11 ton), Toll added!\n");
        }
        break;

         case 9:
        {
          ax3=ax3+1;
          total=total+truck3AXEL;
            printf("\t\t truck(3 axel), Toll added!\n");
        }
        break;

         case 10:
        {
          tra1=tra1+1;
          total=total+ trailer1;
            printf("\t\t trailer(less than 4 axel), Toll added!\n");
        }
        break;

         case 11:
        {
          tra2=tra2+1;
          total=total+ trailer2;
            printf("\t\t trailer(more than 4 axel), Toll added!\n");
        }
        break;
         default:
            printf("\t\t Invalid vihecels\n");

    }

}
while (vehicle!=0);


ArrTotal[i]=total;
totalVehicles=mc+cj+mp+b31+b32+trc5+trc58+trc11+ax3+tra1+tra2;
ArrTotalVehicles[i]=totalVehicles;
}

first = first + 1;
vehicle = 0;
}
void Today(){


        printf("\n--------------------\n");
        printf("Day report\n");
        printf("\t motorcycle=%d\n",mc);
        printf("\t low weight vehicles(car/jeep)=%d\n",cj);
        printf("\t low weight vehicles(micro/pickup)(lower than 1.5 ton)=%d\n",mp);
        printf("\t mini bus(31 seat or less)=%d\n",b31);
        printf("\t big bus(32 srat or more)=%d\n",b32);
        printf("\t small truck(less than 5 ton)=%d\n",trc5);
        printf("\t medium teruck(5-8 ton)=%d\n",trc58);
        printf("\t medium truck(8-11 ton)=%d\n", trc11);
        printf("\t truck(3 axel)=%d\n", ax3);
        printf("\t trailer(less than 4 axel)=%d\n",tra1);
        printf("\t trailer(more than 4 axel)=%d\n",tra2);


        printf("\t...........................\n");
        printf("\t Total Vehicles = %d\n", totalVehicles);
        printf("\t Total Toll money = %.2f TAKA\n", total);


}
void History(){

        for(int i = 0; i < first; i++){

            printf("\t...........................\n");
            printf("date: %d", date[i]);
            printf("\t Total vehicle passed = %d", ArrTotalVehicles[i]);
            printf("\t Total Toll money = %.3f TAKA\n", ArrTotal[i]);

        }
}
void Search(){
        int date1;
        printf("Please enter a date that you want to search: ");
        scanf("%d",&date1);
         printf("\t...........................\n");
        for(int i = 0; i<first; i++){
            if(date1 == date[i]){
            printf("date: %d", date[i]);
            printf("\t Total vehicle passed = %d", ArrTotalVehicles[i]);
            printf("\t Total Toll money = %.2f TAKA\n", ArrTotal[i]);
            }

        }
}


 int main(){

    int option;

    for (;;) {
        printf("\t...........................\n");
        printf("\t\t\tMENU\n");
        printf("Press 1 to start the day\n");
        printf("Press 2 for  day's report\n");
        printf("Press 3 for entire history of the month\n");
        printf("Press 4 to search a specific day report\n");
        printf("Press 0 to exit program\n");
        printf("\t...........................\n");
        printf("Please enter your option here: ");
        scanf("%d",&option);

		switch (option) {
		case 1:
			Add_day();
			break;
		case 2:
			Today();
			break;
        case 3:
            History();
            break;
        case 4:
            Search();
            break;
        case 0:
      //   case 5:
			// exit(0);
      //       break;
		default:
			  printf("\t\t ***********Invalid option*************\n");
			break;
		}
	}


	getch();

 }
