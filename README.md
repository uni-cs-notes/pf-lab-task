# pf-tasks and programming notes 👩‍💻

> prgramming fundamentals lab work &amp; activity

# make a user based program and print the avg of the given values (01)
```
#include <iostream>
using namespace std;
int main(){
    int x,y,z,avg=0;
    cout<<"enter value of x=";
    cin>>x;
    cout<<"enter value of y=";
    cin>>y;
    cout<<"enter value of z=";
    cin>>z;
    avg=(x+y+z)/3;
    cout<<"total avg="<<avg;
    return 0;
  }
```

 # write a user base program based on arthimatics operations (02)
 ```
#include <iostream>
using namespace std;
int main(){
    int x,y,z,a,b,c,d;
    cout<<"enter value of x=";
    cin>>x;
    cout<<"enter value of y=";
    cin>>y;
    cout<<"enter value of z=";
    cin>>z;
    a=x+y;
    b=x-y;
    c=x*y;
    d=x/y;
    cout<<"sum="<<a<<"\n";
    cout<<"submission="<<b<<"\n";
    cout<<"multiple="<<c<<"\n";
    cout<<"division="<<d<<"\n";
    return 0;
}

```

# write a program that takes the radius of cricle from user and print its area (03)
```
#include <iostream>
using namespace std;
int main() {
  float pi=3.14159,r,area=0;
  cout<<"enter radius=";
  cin>>r;
  area=pi*r*r;
  cout<<"area of radius="<<area;
    return 0;
}

```
# create a program that swaps the value of two variables. take the input of two numbers from the user and then swap their values (04)
```
#include <iostream>
using namespace std;
int main() {
    int x, y;
    cout << "Enter the value of x: ";
    cin >> x;
    cout << "Enter the value of y: ";
    cin >> y;

    cout << "Before swapping: x = " << x << ", y = "<< y << "\n";
    a=x;
    x=y;
    y=a;
    cout << "after swapping: x = " << x << ", y = "<< y;
    return 0;
}

```
# make a program to convert temperature from celsius to fahrenheit the user should input the temperature in celsius (05)
```
#include <iostream>
using namespace std;
int main() {
float celsius, fahrenheit;
    cout << "Enter the temperature in Celsius: ";
    cin >> celsius;
    fahrenheit = (celsius * 9/5) + 32;
    cout << "temperature in fahrenhait:" <<fahrenheit;
    return 0;
}
```
# make a program which takes users age & tells them wether user is a child or teen (06)
```
#include <iostream>
using namespace std;
int main() {
int x;
cout<<"enter your age:";
cin>>x;
if (x>=14){
    cout<<"your a teen!"<<endl;
}
    else if (x<14)
    cout<<"your a chlid!"<<endl;

    return 0;
}

```
# make a program that takes to values from the user and swap them with eachother (07)
```
#include <iostream>
using namespace std;
int main() {
int x,y,a;
cout<<"enter the value of x:";
cin>>x;
cout<<"enter the value of y:";
cin>>y;
cout<<"before swappping; x="<<x<<", y= "<<y<<"\n";
a=x;
x=y;
y=a;
cout<<"after swapping; x="<<x<<", y= "<<y<<"\n";
    return 0;
}

```
# swap the values of 2 int by using only 2 variables (08)
```
#include <iostream>
using namespace std;
int main() {
int a=10;
int b=20;
cout<<"before swapping a="<<a<<" ,b="<<b<<"\n";
a=10+20;
b=20-10;
a=30-10;
cout<<"after swapping a="<<a<<" ,b="<<b<<"\n";
    return 0;
}

```
# calculator (09)
```
#include <iostream>
using namespace std;
int main(){
    int num1 , num2 ;
    char keys;
    cout<<"enter your 1st value:";
    cin>>num1;
    cout<<"enter your 2nd value:";
    cin>>num2;
    cout<<"enter your operation:";
    cin>>keys;
    switch (keys){
        case '+': cout<<"answer:"<<(num1+num2); break;
        case '-': cout<<"answer:"<<(num1-num2); break;
        case '*': cout<<"answer:"<<(num1*num2); break;
        case '/': cout<<"answer:"<<(num1/num2); break;
        default : cout<<"invalid operation!!"; break;
    }
  return 0;
}
```
# make a program that ask input in seconds and converts the number into days hour mints and sec value (10)
```
#include <iostream>
using namespace std;
int main(){
int sec,hour,day,mint;
int seconds=0;
cout<<"enter your value in seconds:";
cin>>sec;
day= sec/ (24 * 3600);
hour= (sec% (24 * 3600)) / 3600;
mint= sec % (24 * 3600) / 60;
seconds= (sec % (24 * 3600)) % 60;
cout<<"day:"<<day<<"hour:"<<hour<<"mint:"<<mint<<"sec:"<<seconds;
return 0;
}
```
# make a program that ask for year as an input and tells whather the year is a leap year or not (11)
```
#include <iostream>
using namespace std;
int main(){
int year;
cout<<"enter year:";
cin>>year;
if ((year%4==0) && (year%100!=0))  
    cout<<"ur year is a leap year";
else
    cout<<"ur year is not a leap year";
return 0;
}
```
# make a program that ask for your weight and height and calucalte the BMI (12)
```
#include <iostream>
using namespace std;
int main(){
float weight,height,bmi=0;
cout<<"enter your weight in lb:";
cin>>weight;
cout<<"enter your height in inch:";
cin>>height;
bmi=weight/(height*height)*703;
if (bmi>=18.5 && bmi<=25){
    cout<<"optimal weight    BMI:"<<bmi;
 }
 else if (bmi<18.5){
 cout<<"under weight   BMI:"<<bmi;
} 
else 
 cout<<"over weight   BMI:"<<bmi;
return 0;
}
```
# make a program based on switches that tells the user days of the week (13)
```
#include <iostream>
using namespace std;
int main ()
{
int day;
      cout<<"DAYS OF THE WEEK"<<endl;
      cout<<"1.(sunday)"<<endl;
      cout<<"2.(monday)"<<endl;
      cout<<"3.(tuesday)"<<endl;
      cout<<"4.(wednesday"<<endl;
      cout<<"5.(thursday)"<<endl;
      cout<<"6.(friday)"<<endl;
      cout<<"7.(saturday)"<<endl;
      cout<<"enter the number of the day"<<endl;
      cin>>day;
      switch (day){
          case 1: cout<<"sunday"<<endl;
          break;
          case 2: cout<<"monday"<<endl;
          break;
          case 3: cout<<"tuesday"<<endl;
          break;
          case 4: cout<<"wednesday"<<endl;
          break;
           case 5: cout<<"thursday"<<endl;
          break;
           case 6: cout<<"friday"<<endl;
          break;
           case 7:cout<<"saturday"<<endl;
          break;
          default: cout<<"its not a day!!"<<endl;
          break;
   }
return 0;
 }
```
# make a program that tells the months in a year using switches (14)
```
**#include <iostream>
using namespace std;
int main()
{
    int month;
    cout<<"MONTHS IN A YEAR"<<endl;
    cout<<"1.jan"<<endl;
    cout<<"2.feb"<<endl;
    cout<<"3.march"<<endl;
    cout<<"4.april"<<endl;
    cout<<"5.may"<<endl;
    cout<<"6.june"<<endl;
    cout<<"7.july"<<endl;
    cout<<"8.aug"<<endl;
    cout<<"9.sep"<<endl;
    cout<<"10.oct"<<endl;
    cout<<"11.nov"<<endl;
    cout<<"12.dec"<<endl;
    cout<<"enter ur month number"<<endl;
    cin>>month;
    switch(month){
        case 1: cout <<"jan"<<endl;
        break;
        case 2: cout <<"feb"<<endl;
        break;
        case 3: cout <<"march"<<endl;
        break;
        case 4: cout <<"april"<<endl;
        break;
        case 5: cout <<"may"<<endl;
        break;
        case 6: cout <<"june"<<endl;
        break;
        case 7: cout <<"july"<<endl;
        break;
        case 8: cout <<"aug"<<endl;
        break;
        case 9: cout <<"sep"<<endl;
        break;
        case 10: cout <<"oct"<<endl;
        break;
        case 11: cout <<"nov"<<endl;
        break;
        case 12: cout <<"dec"<<endl;
        break;
    }
}
```
# Write a C++ program that displays a menu with options for different tasks (1 for task A, 2 for task B, etc.). Based on the user's selection, perform the corresponding task using switch case (15)
```
#include <iostream>
using namespace std;
int main()
{
    int task;
    cout<<"following are the tasks"<<endl;
    cout<<"1. task A"<<endl;
    cout<<"2. task B"<<endl;
    cout<<"3. task c"<<endl;
    cout<<"enter your task serial no:"<<endl;
    cin>>task;
    switch (task){
        case 1: cout<<"TASK A"<<endl;
        break;
        case 2: cout<<"TASK B"<<endl;
        break;
        case 3: cout<<"TASK C"<<endl;
        break;
    }
    return 0;
}
```
# loops in c++ [for loop] (16)
```
#include <iostream>

using namespace std;

int main() {
    int i;
    cout<<"enter a value>>>:";
    for (cin >>i;i<=100;i++){
        cout<<i<<endl;
    }
    return 0;
}
```
# loops exapmle in c++ (17)
```
#include <iostream>
using namespace std;
int main()
{
    string s;
   
    cout<<"Press 'y' for Even and 'n' for ODD (y/n) : ";

	cin>> s;
  
    for (int i = 0; i < 100; i++) 
  {
       if(s == "y" || s == "Y")
       {
           	if(i % 2 ==0)
    cout << i <<"  EVEN "<< "\n";
       }
       else if(s == "n" || s == "N")
       {
           if(i % 2 !=0)
    cout << i <<"  ODD "<< "\n";
       }
       else
       {
       cout<< "Invalid";
    break;
           
       }
   
  }

    return 0;
 }
```
# Write a program that takes an integer input from user and displays hollow rectangle of * according to that number (18)
```
#include <iostream>
using namespace std;

int main() {
    int rows, columns;
    int i;
    int j;
    cout << "Enter the number of rows: ";
    cin >> rows;

    cout << "Enter the number of columns: ";
    cin >> columns;

    for( i = 1; i <= rows; i++) {
        for( j = 1; j <= columns; j++) {
            if(i == 1 || i == rows || j == 1 || j == columns) {
                cout << "*";
            } else {
                cout << " ";
            }
        }
        cout << "\n";
    }

    return 0;
}

```
# Nested loop based programs (19) 
```
#include <iostream>
using namespace std;

int main() {
    for (int i = 1; i <= 10; i++) {
        for (int j = 1; j <= 5; j++) {
            cout << i << " x " << j << " = " << i*j << endl;
        }
    }
    return 0;
}
```
# make a pattern of diamond (20)
```
#include <iostream>
using namespace std;
int main() {
    int n;
    cout<<"enter n=";
    cin>>n;
     for (int i=1;i<n;i++){
          for (int j=i;j<=n;j++){
              cout<<" ";
          } for (int j=1;j<=i;j++){
              cout<<"*";
              }
                for (int j=1;j<=i;j++){
                  cout<<"*";
                } 
        cout<<endl;
     }     
       for (int i=1;i<=n;i++){
          for (int j=1;j<=i;j++){
              cout<<" ";
          } for (int j=i;j<=n;j++){
              cout<<"*";
              }
                for (int j=i;j<=n;j++){
                  cout<<"*";
                } 
        cout<<endl;

     }


    return 0;
}
```
# arrays (21)
```
#include <iostream>
#include <string>
using namespace std;

int main()
{
  string cars[4]={ford,honda,bmw,gmc};
   
   cout<<cars[0]<<endl;
   cout<<cars[1]<<endl;
   cout<<cars[2]<<endl;
   cout<<cars[3]<<endl;

   return 0;
}
```
## a better way to write arrays is through loops (22)
```
#include <iostream>
#include <string>
using namespace std;

int main()
{
  string cars[4]={ford,honda,bmw,gmc};
   
for (int i=0;i<4;i++){
    cout<<cars[i];
}

   return 0;
}
```
# making calculator using functions (23)
```
#include <iostream>
#include <string>
#include <cmath>
using namespace std;

 void calculator();
 
int main(){
    calculator();
}

void calculator(){
    float n1,n2;
    cout<<"enter ur 1st interger > ";
      cin >> n1; 
        cout<<"enter ur 2nd interger > ";
         cin >> n2;
    char keys;
     cout<<"enter ur arthimatic operation!>>> ";
       cin>>keys;
    switch (keys){
        case '+': cout<<">"<<n1+n2;
        break;
         case '-': cout<<">"<<n1-n2;
        break;
         case '*': cout<<">"<<n1*n2;
        break;
         case '/': cout<<">"<<n1/n2;
        break;
        default : cout<<"!!!! ERROR !!!!";
        break;
    }
    
}
```

# arrays (21)
```
#include <iostream>
#include <string>
using namespace std;

int main()
{
  string cars[4]={ford,honda,bmw,gmc};
   
   cout<<cars[0]<<endl;
   cout<<cars[1]<<endl;
   cout<<cars[2]<<endl;
   cout<<cars[3]<<endl;

   return 0;
}
```
## a better way to write arrays is through loops (22)
```
#include <iostream>
#include <string>
using namespace std;

int main()
{
  string cars[4]={ford,honda,bmw,gmc};
   
for (int i=0;i<4;i++){
    cout<<cars[i];
}

   return 0;
}
```
# functions (24)
```
#include <iostream>
using namespace std;
void namecall();  //function declearations 
int main(){
    namecall();  //function call
    
}

void namecall(){  //function defination
    string name;
    cout<<"enter ur name >> ";
    cin>>name;
    cout<<name;
}
```
# overload functions (25)
```
#include <iostream>
using namespace std;

// function with 2 parameters
void display(int var1, double var2) {
    cout << "Integer number: " << var1;
    cout << " and double number: " << var2 << endl;
}

// function with double type single parameter
void display(double var) {
    cout << "Double number: " << var << endl;
}

// function with int type single parameter
void display(int var) {
    cout << "Integer number: " << var << endl;
}

int main() {

    int a ;
    double b ;
    
    cout<<"enter ur interger >> ";
    cin>>a;
    cout<<"enter ur double >> ";
    cin>>b;
    
    // call function with int type parameter
    display(a);

    // call function with double type parameter
    display(b);

    // call function with 2 parameters
    display(a, b);

    return 0;
}
```
# 123
```
#include <iostream>
#include <string>
#include <map>
using namespace std;

// Function to register a new user
void registerUser(map<string, string>& users) {
    string username, password;
    cout << "Enter a username: ";
    cin >> username;
    cout << "Enter a password: ";
    cin >> password;

    // Check if the username already exists
    if (users.find(username) != users.end()) {
        cout << "Username already exists. Please choose a different one." << endl;
        return;
    }

    // Create a new user and add it to the map
    users[username] = password;
    cout << "User registered successfully!" << endl;
}

// Function to login a user
void loginUser(map<string, string>& users) {
    string username, password;
    cout << "Enter your username: ";
    cin >> username;
    cout << "Enter your password: ";
    cin >> password;

    // Check if the user exists and the password is correct
    if (users.find(username) != users.end() && users[username] == password) {
        cout << "Login successful!" << endl;
    } else {
        cout << "Invalid username or password." << endl;
    }
}

int main() {
    map<string, string> users;
    int choice;

    do {
        cout << "1. Register\n2. Login\n3. Exit\nEnter your choice: ";
        cin >> choice;

        switch (choice) {
            case 1:
                registerUser(users);
                break;
            case 2:
                loginUser(users);
                break;
            case 3:
                cout << "Goodbye!" << endl;
                break;
            default:
                cout << "Invalid choice. Please try again." << endl;
        }
    } while (choice != 3);

    return 0;
}
```

# zig zag 

>    *       *
>  *  *   *   *
> *      *       *

```

#include <iostream>
using namespace std;

int main(){
  int n = 9;
  for(int i = 1 ; i<=3 ; i++ ){
    for(int j =1 ; j<= n ; j++){
      if(((i+j) % 4 == 0 )||(i == 2 && j % 4 == 0)){
        cout<<"*  ";
      }else 
      cout<< "  ";
    } 
   cout<<endl;
  }
 return 0;
}  

```
# 54321
# 5432
# 543
# 54
# 5

```
#include <iostream>
using namespace std;

int main(){
  int r = 5;
 for(int i = 1 ; i <=r; i++){
     for(int j = r; j >= i ; j--){
         cout<<j<<"";
     }
   cout<<endl;
 }
 return 0;
} 
```

# 5 4 3 2 1 
# 4 3 2 1 
# 3 2 1 
# 2 1 
# 1 
```
#include <iostream>
using namespace std;

int main(){
  int r = 5;
 for(int i = r ; i >= 1; i--){
     for(int j = i; j >= 1 ; j--){
         cout<<j<<" ";
     }
   cout<<endl;
 }
 return 0;
}  
```
# logical programs  

> * 
> * * 
> * * * 
> * * * * 
> * * * * * 

```
#include <iostream>
using namespace std;

int main(){
    int n = 0;
    cout<<"n >> ";
    cin>>n;
    for(int i = 1; i <=n ; i++){
        for(int j = 1; j <= i ; j++){
            cout<<"* ";
        }
      cout<< endl;
    }
 return 0;
}
```

> 1 
> 1 2 
> 1 2 3 
> 1 2 3 4 
> 1 2 3 4 5 

```
#include <iostream>
using namespace std;

int main(){
    int n = 0;
    cout<<"n >> ";
    cin>>n;
    for(int i = 1; i <=n ; i++){
        for(int j = 1; j <= i ; j++){
            cout<<j<<" ";
        }
      cout<< endl;
    }
 return 0;
}
```
> A 
> B B 
> C C C 
> D D D D 
> E E E E E 
> F F F F F F 
```
#include <iostream>
#include <string>
using namespace std;

int main(){
    int n  ;
    cout<<"n >> ";
    cin>>n;
    for(int i = 65; i <=65+n ; i++){
        for(int j = 65; j <= i ; j++){
            cout<<char(i)<<" ";
        }
      cout<< endl;
    }
 return 0;
}
```

> * * * * * 
> * * * * 
> * * * 
> * * 
> * 

```
#include <iostream>
#include <string>
using namespace std;

int main(){
    int n  ;
    cout<<"n >> ";
    cin>>n;
    for(int i = 1 ; i <= n ; i++){
        for(int j = i; j <= n ; j++){
            cout<<"* ";
        }
      cout<< endl;
    }
 return 0;
}
```
> 1 2 3 4 5 
> 1 2 3 4 
> 1 2 3 
> 1 2 
> 1 
```
#include <iostream>
using namespace std;

int main(){
    int n = 0;
    cout<<"n >> ";
    cin>>n;
    for(int i = n ; i >= 1 ; i--){
        for(int j = 1 ; j<= i ; j++){
            cout<<j<<" ";
        }
       cout<< endl;
    }
 return 0;
}
```
>  pyramid  / half diamond  
```
#include <iostream>
using namespace std;

int main(){
  int n = 0;
  cout<<"n > ";
  cin>>n;
  for(int i = 1 ; i <=n ; i++){  
    for(int j = 1 ; j<=n ; j++){ 
      if (j<=n-i){  // j <= n-i so it will print space or else its going to print *
        cout<<" "; 
      } 
      else                  // if j = 1 , n = 5 - i = 1 => 4  (j <=4 true print " ")
       cout<<"* ";    // else j = 1 , n = 5 - i = 5 =>  0  ( * )  
    }
    cout << endl;
  }
  return 0;
}
```
>  HALF  DIAMOND UPSIDE DOWN
> * * * * * 
>  * * * * 
>   * * * 
>    * * 
>     * 

```
#include <iostream>
using namespace std;


int main(){
 int n = 0;
 cout<<"n > ";
 cin>>n;

for(int i = n ; i >=1 ; i--){ 
   for(int j = 1 ; j<=n ; j++){ 
     if (j<=n-i){  
      cout<<" ";
     }
     else                  
    cout<<"* ";    
   }
  cout << endl;
  }
  return 0;
}
```

>     1 
>    1 1 
>   1 2 1 
>  1 3 3 1 
> 1 4 6 4 1 

```
#include <iostream>
using namespace std;

int main(){
 int n = 0;
 cout<<"n > ";
 cin>>n;
  for(int i = 1 ; i<= n ; i++){
       int cofient = 1;
      for(int k = n-i ;k > 0;k--){
          cout<<" ";
      } for( int j = 1 ; j <= i ; j++){
          cout<<cofient<<" ";
          cofient = cofient * (i-j)/j;
      }
      cout<< endl;
  }
return 0;
}
```

> 1 
> 2 3 
> 4 5 6 
> 7 8 9 10 

```
#include <iostream>
using namespace std;

int main(){
    int n = 0;
    cout<<"n >> ";
    cin>>n;
    int num =1;
    for(int i = 1 ; i <=n; i++){
        for(int j = 1; j<=i; j++){
            cout<<num++<<" ";
        }
        cout<<endl;
    }
    return 0;
}

```
## /*1. Write a program in C to store elements in an array and print it.*/
```
#include <iostream>
using namespace std;

int main(){
    int num[5];
    cout<<"enter 5 number >> \n";
    for( int i = 0 ; i < 5 ; i++){
        cin>>num[i];
    } 
    for (int i = 0 ; i < 5 ; i++){
        cout<<"the numbers positions are "<<i<<" >> "<<num[i]<<endl;
    }
  return 0;
}
```
## /*2. Write a program in C to read n number of values in an array and display it in reverse order.*/
```
#include <iostream>
using namespace std;

int main(){
    int n =0;
    cout<<"enter the size of array u want  > ";
    cin>>n;
    int num[n];
    for(int i = 0 ; i < n ; i++){
         cout<<"enter the values for the arrays  >> ";
         cin>>num[i];
    } 

    for(int i= n-1 ; i >=0 ; i--){
        cout<<"the array in reverse order is > "<< num[i]<<endl;
    }
 return 0;
}
```
## /*3. Write a program in C to find the sum of all elements of the array. */
```
#include <iostream>
using namespace std;

int main(){
    int n ; 
    cout<<"the size of array should be > ";
    cin>>n;
    int num[n];
    int sum =0 ;
    for(int i = 0 ; i < n ; i++){
        cout <<"enter the value to the array >> ";
        cin>>num[i];
        sum += num[i];
    }
    cout<<"the sum is > "<< sum << endl;
 return 0;
}
```
## /*4. Write a program in C to copy the elements of one array into another array.*/
```
#include <iostream>
using namespace std;
int main(){
  int n ; 
    cout<<"the size of an array should be > ";
    cin>>n;
    int num[n];
    int num2[n];
    for(int i = 0 ; i < n ; i++){
    cout<<"array 1 >> ";
    cin>>num[i];
    num2[i] = num[i];     
    }
    for(int i = 0 ;i < n ; i++ ){
        cout<<"array 2 >> "<<num2[i]<<endl;
     }
    
 return 0;
}   
```
## /*5. Write a program in C to count a total number of duplicate elements in an array.*/
```
#include <iostream>
using namespace std;
int main(){
    int n ; 
    cout<<"the size of an array should be > ";
    cin>>n;
    int num[n];
    int count =0;
    for(int i = 0 ; i < n ; i++){
    cout<<"array  >> ";
    cin>>num[i];
    }
     for(int i = 0 ; i < n ; i++){
        for(int j = i + 1 ; j < n ; j++){
          if (num[i] == num[j]){
            count++;
          }
        }
    } 
     cout <<"number of duplications > "<< count << endl;
 return 0;
}
```
## /*6. Write a program in C to print all unique elements in an array. */
```
#include <iostream>
using namespace std;

 int main(){
 int n =0;
 cout<<"enter the size of array > ";
 cin>>n;
  char Unielements[n];
  int elements =0 ;
  for(int i = 0 ; i< n ; i++){
  cout<<"enter different number ranging from 30 > 80 input only "<< n-1 <<" amount \n > ";
  cin>> elements;
    (char)elements; //typecasting from int to char
   Unielements[n] = elements;
    cout<<"the elemnts are > "<< Unielements[n] << endl;
  }
  return 0;
}
```
## /*7. Write a program in C to merge two arrays of same size sorted in decending order.*/
```
#include <iostream>
using namespace std;
int main(){
  int arr1[4] = {5,7,9,6};
  int arr2[4] = {4,8,10,1};
  int arr3[8];
  for(int i = 0 ; i < 4 ; i++){
    for(int j = 0 ; j < 4 ; j++){
     arr3[8] = arr1[i] + arr2[j] ;
    }
  } 
return 0;
}
```
## /*9. Write a program in C to find the maximum and minimum element in an array.*/
```
#include <iostream>
using namespace std;

int main(){
  int n =0;
  cout<<"enter the size of an array > ";
  cin>>n;
  int arr[n];
  for(int i = 0 ; i < n ; i++){
    cout <<i+1<<" >> ";
    cin>>arr[i];
  }
  int maxNum = arr[0];
  int minNum = arr[0]; //use the 1st elemnt as starting point for both max and mini numbers 
  for(int i = 1 ; i < n ; i++){
    if (arr[i] > maxNum){
      maxNum = arr[i];
    }
    if (arr[i] < minNum){
        minNum = arr[i];
   }
     
  }    
  cout << "maximum number >> "<<maxNum <<endl;
  cout << "minimum number >> "<<minNum <<endl; 
 return 0;
}
```
## /*10. Write a program in C to separate odd and even integers in separate arrays.*/
```
#include <iostream>
using namespace std;

int main(){
  int arr[8] = {5,9,2,7,65,99,32,1};
  int even[8];
  int odd[8];
  int evenCount , oddCount;

  for(int i = 0 ; i < 8;i++){
    if(arr[i]%2 == 0){
      even[evenCount] = arr[i]; 
      evenCount++;
    }
    if(arr[i]%2 != 0 ){
     odd[oddCount] = arr[i];
     oddCount++;
    }
  }
  for(int i = 0 ; i < evenCount ; i++){
  cout << "even numbers >> "<< even[i] << endl;
  } 
  for(int i = 0 ; i < oddCount ; i++){
  cout << "odd numbers >> "<< odd[i] << endl;
  }
return 0;
}
```
## /*11. Write a program in C to sort elements of array in ascending order.
## 12. Write a program in C to sort elements of the array in descending order.*/
```
#include <iostream>
using namespace std;

int main(){
  int n;
  cout << "Enter the size of the array: ";
  cin >> n;
  int arr[n]; 
  cout << "Enter the array elements:\n";
   for (int i = 0; i < n; i++){
      cin >> arr[i];
    }

    for (int i = 0; i < n - 1; i++){
        for (int j = 0; j < n - i - 1; j++){
            if (arr[j] < arr[j + 1]){ 
                int temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
            }
        }
    }

    
  cout << "Sorted array in descending order: ";
    for (int i = 0; i < n; i++){
      cout << arr[i] << " ";
    }
  cout << endl;

  return 0;
}
```
> // asending order
```
#include <iostream>
using namespace std;

int main(){
    int n;
    cout << "Enter the size of the array > ";
    cin >>n;
    int arr[n]; 
    cout << "Enter the array elements\n";
    for (int i = 0; i < n; i++) {
        cout<<">> ";
        cin >> arr[i];
    }
    for (int i = 0; i < n - 1; i++){
        for (int j = 0; j < n - i - 1; j++){
            if (arr[j] > arr[j + 1]){ 
                int temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
            }
        }
    }
    cout << "Sorted array in ascending order >> ";
    for (int i = 0; i < n; i++){
        cout << arr[i] << " ";
    }
    cout << endl;

    return 0;
}
```
## /*13. Write a program in C to insert New value in the array (sorted list )*/
```
#include <iostream>
using namespace std;

int main() {
    int n;
    cout << "Enter the size of the array > ";
    cin >> n;

    int arr[n + 1];
    cout << "Enter the unsorted array elements \n";
    for (int i = 0; i < n; i++) {
        cin >> arr[i];
    }
    int newValue;
    cout << "Enter the new value to be inserted > ";
    cin >> newValue;

    arr[n] = newValue;

    cout << "Updated array > ";
    for (int i = 0; i <= n; i++){
        cout << arr[i] << " "; 
    }
    cout << endl;

    return 0;
}
```


