# digitalized-menu-card
This project is all about selecting the place you want to visit and the hotels listed in the place can be selected according to your choice,and from the hotel you have selected the list of menus will be given and you can opt according to your choice.
#include<stdio.h>
int cibo();
int blue();
int cascade();
int me();
int dindugal();
int southern();
int hamacho();
int  hilton();
int aman();
int main(){
    int place;
    int choice;
    printf("Choose the location:\n 1.Salem \n 2.Karur \n 3.Tokyo\n");
    scanf("%d",&place);
     switch(place){

         case 1:
             {
                 printf("The hotels available in Salem are listed below:\n\t1.CIBO Restaurant\n\t2.Blue Moon Restaurant\n\t3.The Cascade");
                 printf("\nChoose the restaurant:");
                 scanf("%d",&choice);
                       switch(choice){

                            case 1:
                                {
                                cibo();
                                break;

                              }
                              case 2:
                                  {
                                blue();
                                break;

                              }
                              case 3:
                                  {
                                cascade();
                                break;

                              }

                              default:
                                {
                                    printf("Invalid choice");
                                    break;
                                }
                       }
                 break;

             }

       case 2:
           {
                 printf("The hotels available in Karur are listed below:\n\t1.MEAT AND EAT\n\t2.Dindugal Thalappakatti \n\t3.Southern Spice ");
                 printf("\nChoose the restaurant:");
                 scanf("%d",&choice);
                       switch(choice){

                            case 1:
                                {
                                me();
                                break;

                              }
                              case 2:
                                  {
                                dindugal();
                                break;

                              }
                              case 3:
                                  {
                                southern();
                                break;

                              }

                              default:
                                {
                                    printf("Invalid choice");
                                    break;
                                }
                       }


                 break;

           }

      case 3:
          {
             printf("The hotels available in Tokyo are listed below: \n\t1.Hamacho\n\t2.Hilton\n\t3.Aman");
              printf("\nChoose the restaurant:");
                 scanf("%d",&choice);
                       switch(choice){

                            case 1:
                                {
                                hamacho();
                                break;

                              }
                              case 2:
                                  {
                                hilton();
                                break;

                              }
                              case 3:
                                  {
                                aman();
                                break;

                              }

                              default:
                                {
                                    printf("Invalid choice");
                                    break;
                                }
                       }

                 break;
          }
    default:{
        printf("Invalid choice");
        break;
     }}
     }
int cibo(){

int ch,qty,f;
float itemPrice,totalAmount=0.0;
    printf("\n\tMENU CARD");

    printf("\n\t\t1.MUSHROOM NOODLES     Rs.150+Gst.3 = 153");
    printf("\n\t\t2.BIRIYANI             Rs.100+Gst.2 = 102");
    printf("\n\t\t3.HOT CHILLI PANEER    Rs.210+Gst.5 = 215");
    printf("\n\t\t4.CHEESE GARLIC NAAN   Rs.75+Gst.3 = 78");
    printf("\n\t\t5.CHICKEN TANDOORI     Rs.300+Gst.10 = 310");
    printf("\n\t\t6.CAKE                 Rs.190+Gst.10 = 200");
    printf("\n\t\t7.MUTTON TIKKA         Rs.250+Gst.20 = 270");
    printf("\n\t\t8.JIGARTHANDA          Rs.80+Gst.4 = 84");
    printf("\n\t\t9.MILKSHAKE            Rs.65+Gst.2 = 67");
    printf("\n\t\t10.MOJITO              Rs.65+Gst.3 = 68");
    printf("\n\t\t11.Exit");

     int displayMenu(){
         printf("\n\nEnter Your choice  : ");
         scanf("%d",&ch);
    switch (ch) {
    case 1:
        printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*153;
        return f;
        break;
     case 2:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*102;
         int bri;
        printf("If it is Bakrid or Ramzan click 26:");
        scanf("%d",&bri);
        if(bri==26){
        printf("As it is festival time you are getting 10 percent discount.........");
         f=f-(f*0.10);

     }
        return f;
        break;
     case 3:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*215;
         return f;
        break;
     case 4:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*78;
         return f;
        break;

    case 5:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*310;
         return f;
        break;
   case 6:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*200;
         int chri;
        printf("If it is christmas or newyear click 25:");
        scanf("%d",&chri);
        if(chri==25){
        printf("As it is festival time you are getting 20 percent discount.........");
         f=f-(f*0.20);

     }
         return f;
        break;
    case 7:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*270;
         return f;
        break;
    case 8:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*84;
         return f;
        break;
    case 9:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*67;
         return f;
        break;
    case 10:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*68;
         return f;
        break;

    case 11:
        return 0;
     default:
          printf("\nInvalid Product Selection");
          break;
                }
    }


while ((itemPrice = displayMenu()) != 0) {

        if (itemPrice > 0) {
            totalAmount += itemPrice;
           // printf("Item added to the bill. Current total: $%.2f\n", totalAmount);
        } else if (itemPrice < 0) {
            printf("Error occurred. Exiting...\n");
            return 1;
        } else {
            printf("Thank you for using the Hotel Management System.\n");
        }
    }

    printf("Your total bill is: $%.2f\n", totalAmount);
    printf("THANK YOU FOR VISITING US...........");

    return 0;
}


int blue(){
int ch,qty,f;
float itemPrice,totalAmount=0.0;
    printf("\n\tMENU CARD");

    printf("\n\t\t1.GHEE ROAST        Rs.70+Gst.3= 73.3");
    printf("\n\t\t2.AAPAM             Rs.50+Gst.2 = 52.2");
    printf("\n\t\t3.CHAPATHI          Rs.70+Gst.4 = 74.4");
    printf("\n\t\t4.GOPI MANJURIAN    Rs.75+Gst.3 = 78");
    printf("\n\t\t5.BIRIYANI          Rs.101+Gst.2 = 103");
    printf("\n\t\t6.BUTTER CHICKEN    Rs.190+Gst.10 = 200");
    printf("\n\t\t7.CAKE              Rs.145+Gst.4 = 149");
    printf("\n\t\t8.ICE CREAM         Rs.80+Gst.4 = 84");
    printf("\n\t\t9.POLI              Rs.35+Gst.2 = 37");
    printf("\n\t\t10.RASA GULLA       Rs.65+Gst.3 = 68");
    printf("\n\t\t11.Exit");

     int displayMenu(){
         printf("\n\nEnter Your choice  : ");
         scanf("%d",&ch);
    switch (ch) {
    case 1:
        printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*73.3;
        return f;
        break;
     case 2:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*52.2;

        return f;
        break;
     case 3:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*74.4;
         return f;
        break;
     case 4:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*78;
         return f;
        break;

    case 5:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*103;
         int bri;
        printf("If it is Bakrid or Ramzan click 26:");
        scanf("%d",&bri);
        if(bri==26){
        printf("As it is festival time you are getting 10 percent discount.........");
         f=f-(f*0.10);

     }
         return f;
        break;
   case 6:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*200;
         int chri;
        printf("If it is christmas or newyear click 25:");
        scanf("%d",&chri);
        if(chri==25){
        printf("As it is festival time you are getting 20 percent discount.........");
         f=f-(f*0.20);

     }
         return f;
        break;
    case 7:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*149;
         return f;
        break;
    case 8:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*84;
         return f;
        break;
    case 9:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*37;
         return f;
        break;
    case 10:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*68;
         return f;
        break;

    case 11:
        return 0;
     default:
          printf("\nInvalid Product Selection");
          break;
                }
    }


while ((itemPrice = displayMenu()) != 0) {

        if (itemPrice > 0) {
            totalAmount += itemPrice;
           // printf("Item added to the bill. Current total: $%.2f\n", totalAmount);
        } else if (itemPrice < 0) {
            printf("Error occurred. Exiting...\n");
            return 1;
        } else {
            printf("Thank you for using the Hotel Management System.\n");
        }
    }

    printf("Your total bill is: $%.2f\n", totalAmount);
    printf("THANK YOU FOR VISITING US...........");

    return 0;
}
int cascade(){
int ch,qty,f;
float itemPrice,totalAmount=0.0;
    printf("\n\tMENU CARD");

    printf("\n\t\t1.KADAI PANNER       Rs.150+Gst.3 = 153");
    printf("\n\t\t2.VEG KOLHAPURI      Rs.100+Gst.2 = 102");
    printf("\n\t\t3.BIRIYANI           Rs.210+Gst.5 = 215");
    printf("\n\t\t4.GOBI CHILLI        Rs.75+Gst.3 = 78");
    printf("\n\t\t5.CRAB SOAP          Rs.300+Gst.10 = 310");
    printf("\n\t\t6.CAKE               Rs.190+Gst.10 = 200");
    printf("\n\t\t7.FISH CURRY         Rs.250+Gst.20 = 270");
    printf("\n\t\t8.JUICE              Rs.80+Gst.4 = 84");
    printf("\n\t\t9.MILKSHAKE          Rs.65+Gst.2 = 67");
    printf("\n\t\t10.MOJITO            Rs.65+Gst.3 = 68");
    printf("\n\t\t11.Exit");

     int displayMenu(){
         printf("\n\nEnter Your choice  : ");
         scanf("%d",&ch);
    switch (ch) {
    case 1:
        printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*153;
        return f;
        break;
     case 2:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*102;

        return f;
        break;
     case 3:
         printf("Enter Quantity:");
        scanf("%d",&qty);

        f=qty*215;
         int bri;
        printf("If it is Bakrid or Ramzan click 26:");
        scanf("%d",&bri);
        if(bri==26){
        printf("As it is festival time you are getting 10 percent discount.........");
         f=f-(f*0.10);

     }
         return f;
        break;
     case 4:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*78;
         return f;
        break;

    case 5:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*310;
         return f;
        break;
   case 6:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*200;
         int chri;
        printf("If it is christmas or newyear click 25:");
        scanf("%d",&chri);
        if(chri==25){
        printf("As it is festival time you are getting 20 percent discount.........");
         f=f-(f*0.20);

     }
         return f;
        break;
    case 7:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*270;
         return f;
        break;
    case 8:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*84;
         return f;
        break;
    case 9:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*67;
         return f;
        break;
    case 10:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*68;
         return f;
        break;

    case 11:
        return 0;
     default:
          printf("\nInvalid Product Selection");
          break;
                }
    }


while ((itemPrice = displayMenu()) != 0) {

        if (itemPrice > 0) {
            totalAmount += itemPrice;
           // printf("Item added to the bill. Current total: $%.2f\n", totalAmount);
        } else if (itemPrice < 0) {
            printf("Error occurred. Exiting...\n");
            return 1;
        } else {
            printf("Thank you for using the Hotel Management System.\n");
        }
    }

    printf("Your total bill is: $%.2f\n", totalAmount);
    printf("THANK YOU FOR VISITING US...........");

    return 0;
}
int me(){
int ch,qty,f;
float itemPrice,totalAmount=0.0;
    printf("\n\tMENU CARD");

    printf("\n\t\t1.MUSHROOM NOODLES     Rs.150+Gst.3 = 153");
    printf("\n\t\t2.BIRIYANI             Rs.100+Gst.2 = 102");
    printf("\n\t\t3.HOT CHILLI PANEER    Rs.210+Gst.5 = 215");
    printf("\n\t\t4.CHEESE GARLIC NAAN   Rs.75+Gst.3 = 78");
    printf("\n\t\t5.CHICKEN TANDOORI     Rs.300+Gst.10 = 310");
    printf("\n\t\t6.CAKE                 Rs.190+Gst.10 = 200");
    printf("\n\t\t7.PRAWN CURRY          Rs.250+Gst.20 = 270");
    printf("\n\t\t8.JIGARTHANDA          Rs.80+Gst.4 = 84");
    printf("\n\t\t9.MILKSHAKE            Rs.65+Gst.2 = 67");
    printf("\n\t\t10.MOJITO              Rs.65+Gst.3 = 68");
    printf("\n\t\t11.Exit");

     int displayMenu(){
         printf("\n\nEnter Your choice  : ");
         scanf("%d",&ch);
    switch (ch) {
    case 1:
        printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*153;
        return f;
        break;
     case 2:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*102;
        int bri;
        printf("If it is Bakrid or Ramzan click 26:");
        scanf("%d",&bri);
        if(bri==26){
        printf("As it is festival time you are getting 10 percent discount.........");
         f=f-(f*0.10);

     }
        return f;
        break;
     case 3:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*215;
         return f;
        break;
     case 4:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*78;
         return f;
        break;

    case 5:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*310;
         return f;
        break;
   case 6:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*200;
         int chri;
        printf("If it is christmas or newyear click 25:");
        scanf("%d",&chri);
        if(chri==25){
        printf("As it is festival time you are getting 20 percent discount.........");
         f=f-(f*0.20);

     }
         return f;
        break;
    case 7:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*270;
         return f;
        break;
    case 8:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*84;
         return f;
        break;
    case 9:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*67;
         return f;
        break;
    case 10:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*68;
         return f;
        break;

    case 11:
        return 0;
     default:
          printf("\nInvalid Product Selection");
          break;
                }
    }


while ((itemPrice = displayMenu()) != 0) {

        if (itemPrice > 0) {
            totalAmount += itemPrice;
           // printf("Item added to the bill. Current total: $%.2f\n", totalAmount);
        } else if (itemPrice < 0) {
            printf("Error occurred. Exiting...\n");
            return 1;
        } else {
            printf("Thank you for using the Hotel Management System.\n");
        }
    }

    printf("Your total bill is: $%.2f\n", totalAmount);
    printf("THANK YOU FOR VISITING US...........");

    return 0;
}
int dindugal(){
int ch,qty,f;
float itemPrice,totalAmount=0.0;
    printf("\n\tMENU CARD");

    printf("\n\t\t1.MUSHROOM NOODLES     Rs.150+Gst.3 = 153");
    printf("\n\t\t2.BIRIYANI             Rs.100+Gst.2 = 102");
    printf("\n\t\t3.HOT CHILLI PANEER    Rs.210+Gst.5 = 215");
    printf("\n\t\t4.CHEESE GARLIC NAAN   Rs.75+Gst.3 = 78");
    printf("\n\t\t5.CHICKEN TANDOORI     Rs.300+Gst.10 = 310");
    printf("\n\t\t6.CAKE                 Rs.190+Gst.10 = 200");
    printf("\n\t\t7.PRAWN CURRY          Rs.250+Gst.20 = 270");
    printf("\n\t\t8.JIGARTHANDA          Rs.80+Gst.4 = 84");
    printf("\n\t\t9.MILKSHAKE            Rs.65+Gst.2 = 67");
    printf("\n\t\t10.MOJITO              Rs.65+Gst.3 = 68");
    printf("\n\t\t11.Exit");

     int displayMenu(){
         printf("\n\nEnter Your choice  : ");
         scanf("%d",&ch);
    switch (ch) {
    case 1:
        printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*153;
        return f;
        break;
     case 2:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*102;
        int bri;
        printf("If it is Bakrid or Ramzan click 26:");
        scanf("%d",&bri);
        if(bri==26){
        printf("As it is festival time you are getting 10 percent discount.........");
         f=f-(f*0.10);

     }
        return f;
        break;
     case 3:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*215;
         return f;
        break;
     case 4:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*78;
         return f;
        break;

    case 5:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*310;
         return f;
        break;
   case 6:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*200;
         int chri;
        printf("If it is christmas or newyear click 25:");
        scanf("%d",&chri);
        if(chri==25){
        printf("As it is festival time you are getting 20 percent discount.........");
         f=f-(f*0.20);

     }
         return f;
        break;
    case 7:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*270;
         return f;
        break;
    case 8:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*84;
         return f;
        break;
    case 9:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*67;
         return f;
        break;
    case 10:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*68;
         return f;
        break;

    case 11:
        return 0;
     default:
          printf("\nInvalid Product Selection");
          break;
                }
    }


while ((itemPrice = displayMenu()) != 0) {

        if (itemPrice > 0) {
            totalAmount += itemPrice;
           // printf("Item added to the bill. Current total: $%.2f\n", totalAmount);
        } else if (itemPrice < 0) {
            printf("Error occurred. Exiting...\n");
            return 1;
        } else {
            printf("Thank you for using the Hotel Management System.\n");
        }
    }

    printf("Your total bill is: $%.2f\n", totalAmount);
    printf("THANK YOU FOR VISITING US...........");

    return 0;
}
int southern(){
int ch,qty,f;
float itemPrice,totalAmount=0.0;
    printf("\n\tMENU CARD");

    printf("\n\t\t1.MUSHROOM NOODLES     Rs.150+Gst.3 = 153");
    printf("\n\t\t2.BIRIYANI             Rs.100+Gst.2 = 102");
    printf("\n\t\t3.HOT CHILLI PANEER    Rs.210+Gst.5 = 215");
    printf("\n\t\t4.CHEESE GARLIC NAAN   Rs.75+Gst.3 = 78");
    printf("\n\t\t5.CHICKEN TANDOORI     Rs.300+Gst.10 = 310");
    printf("\n\t\t6.CAKE                 Rs.190+Gst.10 = 200");
    printf("\n\t\t7.PRAWN CURRY          Rs.250+Gst.20 = 270");
    printf("\n\t\t8.JIGARTHANDA          Rs.80+Gst.4 = 84");
    printf("\n\t\t9.MILKSHAKE            Rs.65+Gst.2 = 67");
    printf("\n\t\t10.MOJITO              Rs.65+Gst.3 = 68");
    printf("\n\t\t11.Exit");

     int displayMenu(){
         printf("\n\nEnter Your choice  : ");
         scanf("%d",&ch);
    switch (ch) {
    case 1:
        printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*153;
        return f;
        break;
     case 2:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*102;
        int bri;
        printf("If it is Bakrid or Ramzan click 26:");
        scanf("%d",&bri);
        if(bri==26){
        printf("As it is festival time you are getting 10 percent discount.........");
         f=f-(f*0.10);

     }
        return f;
        break;
     case 3:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*215;
         return f;
        break;
     case 4:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*78;
         return f;
        break;

    case 5:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*310;
         return f;
        break;
   case 6:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*200;
         int chri;
        printf("If it is christmas or newyear click 25:");
        scanf("%d",&chri);
        if(chri==25){
        printf("As it is festival time you are getting 20 percent discount.........");
         f=f-(f*0.20);

     }
         return f;
        break;
    case 7:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*270;
         return f;
        break;
    case 8:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*84;
         return f;
        break;
    case 9:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*67;
         return f;
        break;
    case 10:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*68;
         return f;
        break;

    case 11:
        return 0;
     default:
          printf("\nInvalid Product Selection");
          break;
                }
    }


while ((itemPrice = displayMenu()) != 0) {

        if (itemPrice > 0) {
            totalAmount += itemPrice;
           // printf("Item added to the bill. Current total: $%.2f\n", totalAmount);
        } else if (itemPrice < 0) {
            printf("Error occurred. Exiting...\n");
            return 1;
        } else {
            printf("Thank you for using the Hotel Management System.\n");
        }
    }

    printf("Your total bill is: $%.2f\n", totalAmount);
    printf("THANK YOU FOR VISITING US...........");

    return 0;
}
int hamacho(){
int ch,qty,f;
float itemPrice,totalAmount=0.0;
    printf("\n\tMENU CARD");

    printf("\n\t\t1.TAMAGEYAKI           Rs.150+Gst.3 = 153");
    printf("\n\t\t2.UNAGI                Rs.100+Gst.2 = 102");
    printf("\n\t\t3.SASHIMI              Rs.210+Gst.5 = 215");
    printf("\n\t\t4.KASHIPAN             Rs.75+Gst.3 = 78");
    printf("\n\t\t5.GYOZA                Rs.300+Gst.10 = 310");
    printf("\n\t\t6.CAKE                 Rs.190+Gst.10 = 200");
    printf("\n\t\t7.ULAGYU BEEF          Rs.250+Gst.20 = 270");
    printf("\n\t\t8.MIRO SOUP            Rs.80+Gst.4 = 84");
    printf("\n\t\t9.OKONOMIYAKI          Rs.65+Gst.2 = 67");
    printf("\n\t\t10.MIKUJAGA            Rs.65+Gst.3 = 68");
    printf("\n\t\t11.Exit");

     int displayMenu(){
         printf("\n\nEnter Your choice  : ");
         scanf("%d",&ch);
    switch (ch) {
    case 1:
        printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*153;
        return f;
        break;
     case 2:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*102;
        return f;
        break;
     case 3:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*215;
         return f;
        break;
     case 4:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*78;
         return f;
        break;

    case 5:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*310;
         return f;
        break;
   case 6:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*200;
         int chri;
        printf("If it is christmas or newyear click 25:");
        scanf("%d",&chri);
        if(chri==25){
        printf("As it is festival time you are getting 20 percent discount.........");
         f=f-(f*0.20);

     }
         return f;
        break;
    case 7:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*270;
         return f;
        break;
    case 8:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*84;
         return f;
        break;
    case 9:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*67;
         return f;
        break;
    case 10:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*68;
         return f;
        break;

    case 11:
        return 0;
     default:
          printf("\nInvalid Product Selection");
          break;
                }
    }


while ((itemPrice = displayMenu()) != 0) {

        if (itemPrice > 0) {
            totalAmount += itemPrice;
           // printf("Item added to the bill. Current total: $%.2f\n", totalAmount);
        } else if (itemPrice < 0) {
            printf("Error occurred. Exiting...\n");
            return 1;
        } else {
            printf("Thank you for using the Hotel Management System.\n");
        }
    }

    printf("Your total bill is: $%.2f\n", totalAmount);
    printf("THANK YOU FOR VISITING US...........");

    return 0;
}
int hilton(){
int ch,qty,f;
float itemPrice,totalAmount=0.0;
    printf("\n\tMENU CARD");

    printf("\n\t\t1.SUSHI                Rs.150+Gst.3 = 153");
    printf("\n\t\t2.SUKIYAKI             Rs.100+Gst.2 = 102");
    printf("\n\t\t3.RAMEN                Rs.210+Gst.5 = 215");
    printf("\n\t\t4.BUBBLE TEA           Rs.75+Gst.3 = 78");
    printf("\n\t\t5.TEMPURA              Rs.300+Gst.10 = 310");
    printf("\n\t\t6.CAKE                 Rs.190+Gst.10 = 200");
    printf("\n\t\t7.ODEN                 Rs.250+Gst.20 = 270");
    printf("\n\t\t8.ONIGIRI              Rs.80+Gst.4 = 84");
    printf("\n\t\t9.TSUKEMEN             Rs.65+Gst.2 = 67");
    printf("\n\t\t10.UNAGI               Rs.65+Gst.3 = 68");
    printf("\n\t\t11.Exit");

     int displayMenu(){
         printf("\n\nEnter Your choice  : ");
         scanf("%d",&ch);
    switch (ch) {
    case 1:
        printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*153;
        return f;
        break;
     case 2:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*102;
        return f;
        break;
     case 3:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*215;
         return f;
        break;
     case 4:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*78;
         return f;
        break;

    case 5:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*310;
         return f;
        break;
   case 6:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*200;
         int chri;
        printf("If it is christmas or newyear click 25:");
        scanf("%d",&chri);
        if(chri==25){
        printf("As it is festival time you are getting 20 percent discount.........");
         f=f-(f*0.20);

     }
         return f;
        break;
    case 7:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*270;
         return f;
        break;
    case 8:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*84;
         return f;
        break;
    case 9:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*67;
         return f;
        break;
    case 10:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*68;
         return f;
        break;

    case 11:
        return 0;
     default:
          printf("\nInvalid Product Selection");
          break;
                }
    }


while ((itemPrice = displayMenu()) != 0) {

        if (itemPrice > 0) {
            totalAmount += itemPrice;
           // printf("Item added to the bill. Current total: $%.2f\n", totalAmount);
        } else if (itemPrice < 0) {
            printf("Error occurred. Exiting...\n");
            return 1;
        } else {
            printf("Thank you for using the Hotel Management System.\n");
        }
    }

    printf("Your total bill is: $%.2f\n", totalAmount);
    printf("THANK YOU FOR VISITING US...........");

    return 0;
}
int aman(){
int ch,qty,f;
float itemPrice,totalAmount=0.0;
    printf("\n\tMENU CARD");

    printf("\n\t\t1.TENDON               Rs.150+Gst.3 = 153");
    printf("\n\t\t2.NATTO                Rs.100+Gst.2 = 102");
    printf("\n\t\t3.GYOZA                Rs.210+Gst.5 = 215");
    printf("\n\t\t4.TOFU CURRY           Rs.75+Gst.3 = 78");
    printf("\n\t\t5.ODEN                 Rs.300+Gst.10 = 310");
    printf("\n\t\t6.CAKE                 Rs.190+Gst.10 = 200");
    printf("\n\t\t7.MENTAIKO             Rs.250+Gst.20 = 270");
    printf("\n\t\t8.TONKASTU             Rs.80+Gst.4 = 84");
    printf("\n\t\t9.MONJAYAKI            Rs.65+Gst.2 = 67");
    printf("\n\t\t10.DONBURI             Rs.65+Gst.3 = 68");
    printf("\n\t\t11.Exit");

     int displayMenu(){
         printf("\n\nEnter Your choice  : ");
         scanf("%d",&ch);
    switch (ch) {
    case 1:
        printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*153;
        return f;
        break;
     case 2:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*102;
        return f;
        break;
     case 3:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*215;
         return f;
        break;
     case 4:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*78;
         return f;
        break;

    case 5:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*310;
         return f;
        break;
   case 6:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*200;
         int chri;
        printf("If it is christmas or newyear click 25:");
        scanf("%d",&chri);
        if(chri==25){
        printf("As it is festival time you are getting 20 percent discount.........");
         f=f-(f*0.20);

     }
         return f;
        break;
    case 7:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*270;
         return f;
        break;
    case 8:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*84;
         return f;
        break;
    case 9:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*67;
         return f;
        break;
    case 10:
         printf("Enter Quantity:");
        scanf("%d",&qty);
        f=qty*68;
         return f;
        break;

    case 11:
        return 0;
     default:
          printf("\nInvalid Product Selection");
          break;
                }
    }


while ((itemPrice = displayMenu()) != 0) {

        if (itemPrice > 0) {
            totalAmount += itemPrice;

        } else if (itemPrice < 0) {
            printf("Error occurred. Exiting...\n");
            return 1;
        } else {
            printf("Thank you for using the Hotel Management System.\n");
        }
    }
    printf("Your total bill is: $%.2f\n", totalAmount);
    printf("THANK YOU FOR VISITING US...........");

    return 0;
}
