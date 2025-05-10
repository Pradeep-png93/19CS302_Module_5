# EX 24 : CREATE A STRUCTURE PROGRAM TO READ(EMPNO,DEPT AND BASIC PAY) AND STORE THE DATA OF 3 EMPLOYEES AND CALCULATE THEIR GROSS SALARY
## AIM:
To Create a structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary(da =10% and HRA=30% from BP).

## Algorithm
1.	Start.
2.	Define a variables.
3.	Create a structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary(da =10% and HRA=30% from BP).
4.	Read the value using scanf.
5.	Ask the user to make an input.
6.	Print out the answer.
7.	End.

## Program:
```
OGRAM:
#include <stdio.h>
struct Employee {
int empno;
char dept[100];
float basic_pay;
float gross_salary;
float da;
float hra;
};
int main() {
struct Employee employees[3];
for (int i = 0; i < 3; ++i) {
scanf("%d", &employees[i].empno);
scanf("%s", employees[i].dept);
scanf("%f", &employees[i].basic_pay);
employees[i].da = 0.1 * employees[i].basic_pay; // DA is 10% of Basic Pay
employees[i].hra = 0.3 * employees[i].basic_pay; // HRA is 30% of Basic Pay
employees[i].gross_salary = employees[i].basic_pay + employees[i].da +
employees[i].hra;
}
printf("Details of the Employee:\n");
SAVEETHA ENGINEERING COLLEGE
for (int i = 0; i < 3; ++i) {
printf("%d %s %.f %.f %.f %.2f\n", employees[i].empno, employees[i].dept,
employees[i].basic_pay, employees[i].da, employees[i].hra, employees[i].gross_salary);
}
return 0;
}

```

## Output:

![image](https://github.com/user-attachments/assets/5659af78-5ba1-4be7-a4fa-5740903b972f)


## Result:
Thus the program was executed and the output was verified successfully.
