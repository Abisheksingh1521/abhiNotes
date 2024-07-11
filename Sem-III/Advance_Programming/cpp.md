# C++

 You are given two strings, a, and b, separated by a new line. Each 
string will consist of lower case alphabets. In the first line print two 
space-separated integers, representing the length of a and b 
respectively. In the second line print the string produced by 
concatenating a and b. In the third line print two strings separated 
by a space, al and bl. al and bl are the same as a and b, respectively, 
except that their first characters are swapped. 

```cpp

#include<iostream>
#include<string>
using namespace std;
int main()
{
	string a,b;
	cout<<"enter string a :"<<endl;
	cin>>a;
	cout<<"enter string b:"<<endl;
	cin>>b;
	cout<<"the length of a and b is:"<<a.length()<<" "<<b.length()<<endl;
	cout<<a+b<<endl;
	swap(a[0],b[0]);
	cout<<a;
		
}
```
#### We can store details related to a student in a class consisting of his 
age (int), first_name (string), last_name (string) and standard (int). 
You must create a class, named Student, representing the student's 
details, as mentioned above, and store the data of a student. 
Create setter and getter functions for each element; that is, the 
class should at least have following functions: get_age, set_age 
get_first_name, set_first_name get_last_name, set_last_name 
get_standard, set_standard

```cpp
#include<iostream>
#include<string> using
namespace std; class
student{
int age,standard;
string first_name,last_name;
public:
void set_age(){
cout<<"enter the age of the student"<<endl; cin>>age;
}
void get_age(){
cout<<"Age:"<<age<<endl;
}
void set_first_name(){
cout<<"enter the first name of the student"<<endl;
cin>>first_name;
}
void get_first_name(){
cout<<"First name:"<<first_name<<endl;
}
void set_last_name(){
cout<<"enter the last name of the student"<<endl;
cin>>last_name;
}
void get_last_name(){
cout<<"Last name:"<<last_name<<endl;
}
void set_standard(){
cout<<"enter the standard of the student"<<endl;
cin>>standard;
}
void get_standard(){
cout<<"Standard:"<<standard<<"th"<<endl;
}
};
int main(){
student s;
s.set_first_name();
s.set_last_name();
s.set_age();
s.set_standard();
s.get_first_name();
s.get_last_name();
s.get_age();
s.get_standard();
return 0;
}
```

#### Create the student class with the following data members:
student_name, roll_num, marks1, marks2. Take name, roll number,
marks1 and marks2 information from user. Calculate the mean value
of marks and display student_name, roll_num, mean mark values.

``` cpp
#include<iostream>
#include<string>
using namespace std;
class student{
string student_name;
int roll_no,mark1,mark2;
float mean;
public:
void set(){
cout<<"enter the name of the student"<<endl;
cin>>student_name;
cout<<"enter the roll no"<<endl;
cin>>roll_no;
cout<<"enter the Mark 1"<<endl;
cin>>mark1;
cout<<"enter the Mark 2"<<endl;
cin>>mark2;
mean=(mark1+mark2)/2;
}
void get(){
cout<<"Name:"<<student_name<<endl;
cout<<"Roll No:"<<roll_no<<endl;
cout<<"Mark in Subject 1:"<<mark1<<endl;
cout<<"Mark in Subject 2:"<<mark2<<endl;
cout<<"Mean mark:"<<mean<<endl;
}
};
int main(){
student s;
s.set();
s.get();
}

```
#### Create the Worker class mentioning theirid, name, and group (A or B or
C) to which they belong. Compute their weekly wagesfor the number of
hoursthey work, fixing a nominal pay rate which is a sensitive data.
Include the Accessor and mutator member functionsto set and display
the wages.

```cpp
#include<iostream>
#include<string>
using namespace std;
class workers{
int id,hours;
string name,group;
float wage;
public:
void input(){
int amt=300;
cout<<"enter the name of the worker"<<endl;
cin>>name;
cout<<"enter the woker id"<<endl;
cin>>id;
cout<<"enter the group"<<endl;
cin>>group;
cout<<"enter the numbers of hours worked"<<endl;
cin>>hours;
wage=amt*hours;
}
void output(){
cout<<"Name of the worker: "<<name<<endl;
cout<<"Worker ID: "<<id<<endl;
cout<<"Group: "<<group<<endl;
cout<<"Number of hours worked: "<<hours<<endl;
cout<<"Total wage: "<<wage<<endl;
}
};
int main(){
workers w;
w.input();
w.output();
}
```
#### Solve above Ǫuestion number with 'n' workers using array of objects
```cpp
#include<iostream>
#include<string>
using namespace std;
class workers{
int id,hours;
string name,group;
float wage;
public:
void input(){
int amt=300;
cout<<"enter the name of the worker"<<endl;
cin>>name;
cout<<"enter the woker id"<<endl;
cin>>id;
cout<<"enter the group"<<endl;
cin>>group;
cout<<"enter the numbers of hours worked"<<endl;
cin>>hours;
wage=amt*hours;
}
void output(){
cout<<"Name of the worker: "<<name<<endl;
cout<<"Worker ID: "<<id<<endl;
cout<<"Group: "<<group<<endl;
cout<<"Number of hours worked: "<<hours<<endl;
cout<<"Total wage: "<<wage<<endl;
}
};
int main(){
int n;
cout<<"enter the number of workers: "<<endl;
cin>>n;
workers w[n];
for(inti=0;i<n;i++){
cout<<"Enter the details of worker "<<i+1<<":"<<endl;
w[i].input();
}
for(int i=0;i<n;i++){
cout<<"Details and wage of worker "<<i+1<<":"<<endl;
w[i].output();
}
}
```
#### Kristen is a contender for valedictorian of her high school. She wants to know how many
students (if any) have scored higher than her in the 5 exams given during this semester.
Create a class named Student with the following specifications:
An instance variable named scores to hold a student's 5 exam scores.
A void input() function that reads 5 integers and saves them to scores.
An int calculateTotalScore() function that returns the sum of the student's scores.
```cpp
#include<iostream>
using namespace std;
class student{
int score[4];
public:
void input(){
for(int j=0;j<4;j++){
cout<<"enter the mark "<<j+1<<endl;
cin>>score[j];
}
}
int totalscore(){
int total=0;
for(int j=0;j<4;j++){
cout<<"Mark
"<<j+1<<"="<<score[j]<<endl;
total=total+score[j];
}
cout<<"Total marks :"<<total<<endl;
}
};
int
main(
){ int
i,n;
cout<<"enter the no of
students"<<endl; cin>>n;
student s[n];
for( i=0;i<n;i++){
cout<<"enter the marks of student "<<i+1<<endl;
s[i].input();
}
for( i=0;i<n;i++){
cout<<"marks of student "<<i+1<<endl;
s[i].totalscore();
}
}
```





