# Wind-Chill-Factor-Calculator
This program calculates the wind chill factor using the standard wind chill formula, which combines air temperature and wind velocity to estimate the perceived cold. It takes temperature and wind velocity as user inputs via scanf, computes the result using pow() from math.h, and displays the wind chill factor.

#include <stdio.h>
#include <math.h>

int main (){

float wcf, t, v;

printf("Enter the value of Temprature");
scanf("%f", &t);

printf("Enter the value of Wind Velocity");
scanf("%f", &v);

wcf=35.74+0.6215*t+(0.4275*t-35.75)*pow(v,0.16);

printf("Wind Chill factor is=%f",wcf);

return 0;

}
