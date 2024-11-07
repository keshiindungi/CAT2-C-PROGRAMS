#include <stdio.h>

int main(){
    float hoursWorked, hourlyWage, grossPay, tax, netPay;
    
    printf("Enter hours worked: \n");
    scanf("%f", &hoursWorked);
    printf("Enter hourly wage: \n");
    scanf("%f", &hourlyWage);
    
    if (hoursWorked > 40){
        //Regular pay for 40 hours
        float regularPay = 40 * hourlyWage;
        float overtimeHours = hoursWorked - 40;
        float overtimePay = overtimeHours * hourlyWage * 1.5;
        //Total gross pay
        grossPay = regularPay + overtimePay;
    } else {
        grossPay = hoursWorked * hourlyWage;
    }
    
    //Calculate taxes
    if (grossPay <= 600){
        tax = grossPay * 0.15;
    } else {
        tax = (600 * 0.15) + ((grossPay - 600) * 0.20);
    }
    
    //Calculate net pay
    netPay = grossPay - tax;
    

    printf("Gross Pay: $%.2f\n", grossPay);
    printf("Taxes: $%.2f\n", tax);
    printf("Net Pay: $%.2f\n", netPay);
    
    return 0;

    
}