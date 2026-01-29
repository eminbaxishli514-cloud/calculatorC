This readme will explain a very simple calculator that was written in C.


/*A simple calculator written in C*/
#include <stdio.h>
#include <stdlib.h>

double sum(double a,double b){
    return a+b;
}

double multiply(double a,double b){
    return a*b;

}
double subtract(double a,double b){
    return a-b;


}
double divide(double a,double b){
    return a/b;

} This part just defines the functions as we did in python.



int main(){
    double first_number;
    double second_number;
    char op;
    printf("Enter the first number: ");
    scanf("%lf",&first_number);
    printf("Enter the second number: ");
    scanf("%lf",&second_number);
    printf("Which operation would you like to perform?(+-*/)");
    scanf(" %c",&op);
    if (op== '+'){
        printf("%f",sum(first_number,second_number));
    }else if(op== '-'){
        printf("%f",subtract(first_number,second_number));
    }else if(op=='*'){
        printf("%f",multiply(first_number,second_number));

    }else if(op=='/'){
        if (second_number!=0){
            printf("%f",divide(first_number,second_number));
        }else{

            printf("You can not divide by zero");

        }


    }else{
        printf("The operator you entered is invalid");
    }


    return 0;  

  In this part, we just initiate the variables and specifiy their types and utilize scanf to take the user input and based on the operator, correct operations are done

  
