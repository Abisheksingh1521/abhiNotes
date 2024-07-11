# C++

#### You are given two strings, a, and b, separated by a new line. Each 
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



