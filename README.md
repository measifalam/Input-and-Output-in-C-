# Input-and-Output-in-C-
Input and output are critical pieces of C++ programs (or any program). In C++, input/output (I/O) is handled through streams, which are really modes of data transmission. The class iostream supports I/O operations. The key child classes for input are cin, and for output the class is cout.

// 1.Display a message using pre-defined objects
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
#include<iostream>
using namespace std;

int main()
{
 
 cout<<"\n measifalam doing things"; 
 cerr<<"\n measifalam doing things"; 
 clog<<"\n measifalam doing things"; 
return 0;
}

=================================================================

//2. Display
~~~~~~~~~~~~~~~
#include<iostream>
using namespace std;

int main()
{
 cout<<"measifalam";
 return 0;
}

====================================================================


//3. Display
~~~~~~~~~~~~~~~
#include<iostream>
using namespace std;

int main()
{
char *n="measifalam";
cout<<n;
return 0;
}

=================================================================
//4. Display
~~~~~~~~~~~~~~~
#include<iostream>
using namespace std;

int main()
{
int x=10;
float f=3.14;
cout<<x;
cout<<"\t";
cout<<f;
return 0;
}

=================================================================
//5.Accept  string through Keyboard & display
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
#include<iostream>
using namespace std;

int main()
{
char name[15];
cout<<"Enter username";
cin>>name;
cout<<"User is";
cout<<name;
return 0;
}

====================================================================
//6. Read two integer and display
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
#include<iostream>
using namespace std;

int main()
{
int a,b;
cout<<"Enter the 1st number";
cin>>a;
cout<<"Enter the 2nd number";
cin>>b;
cout<<"Entered numbers are";
cout<<a<<"\t"<<b;

return 0;
}

=====================================================================
7.Program to display data using cout
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
int main()
{
cout<<"Hello ";
cout<<"It's ";
cout<<"measif";
cout<<"alam";
cout<<"doing";
cout<<"things.";
return 0;
}


=====================================================================
8.To display int,float,char and string using cout statements
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#include<iostream>
using namespace std;

int main()
{
int a=2020;
float b=20.20;
char c='A';
string d="measifalam";
cout<<"a="<<a;
cout<<"b="<<b;
cout<<"c="<<c;
cout<<"d="<<d;

return 0;
}

===============================================================

//9.To input & display int,float,char and string using cout statements
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#include<iostream>
using namespace std;

int main()
{
int i;
float f;
char c;
char s[15] ;
cout<<"\n Enter the integer";
cin>>i;
cout<<"\n Enter the float";
cin>>f;
cout<<"\n Enter the character:'
cin>>c;
cout<<"\n Enter the string";
cin>>s;

cout<<"\nEntered values";
cout<<i<<"\n";
cout<<f<<"\n";
cout<<c<<"\n";
cout<<s<<"\n";

return 0;
}

====================================================

//10.Applying diffirent format of typecasting and display
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#include<iostream>
using namespace std;

int main()
{
 int a=66;
 float f=2.5;
 double d=85.22;
 char c='K';
 
 cout<<"\n int in char format:"<<(char)a;
 cout<<"\n float in int format:"<<(int)f;
 cout<<"\n double in char format:"<<(char)d;
 cout<<'\n char in int format:"<<(int)c;
 return 0;
}

==============================================

//11.Display data using typecasting
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~`

#include<iostream>
using namespace std;

int main()
{
int a=90;
float b=15.256;
char c='Z';
cout<<"a="<<(char)a;
cout<<"b="<<(int)b;
cout<<"c="<<(int)c;
return 0;

}

==============================================
//12.Program to deisplay alphabets

#include<iostream>
#include<stdio.h>
using namespace std;

int main()
{
  for(int j=0;j<91;j++)
    {
cout<<(char)j<<" ";
    }

cout<<endl;

  for(int j=0;j<91;j++)
  {
   printf("%c",j);
  }
  
  return 0;
}

===============================================

//13.For displaying addresses of variables in hexadecimal and unsigned integer
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#include<iostream>
using namespace std;

int main()
{
 int a=66;
 float f=2.5;
 double d=85.22;
 char c='K';
 cout<<"Address of a:"<<&x<<endl;
 cout<<"Address of f:"<<&f<<endl;
 cout<<"Address of d:"<<&d<<(unsigned)endl;
 
 return 0;
 }
 
 ============================================
 
 //14.Display string string using & and * operator
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 #include<iostream>
 using namespace std;
 
 int main()
 {
 char *name="me  asif alam";
 cout<<name<<"\n;
 cout<<&name[0]<<"\n";
 cout<<*(&name);
 return 0;
}

=======================================

//15.Display character on the screen using put() function
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
#include<iostream>
using namespace std;

int main()
{
cout.put('1');
cout.put('2');
cout.put('3');
return 0;
}

============================================

//16.To use escape sequence with cout.put() statement
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#include<iostream>
using namespace std;

int main()
{
cout.put('1');
cout.put('\n');
cout.put('2');
return 0;
}

====================================

//18.use multiple put statement
~~~~~~~~~~~~~~~~~~~~~~~~~~~
#include<iostream>
using namespace std;

int main()
{
 cout.put('A').put('B').put('C');
 return 0;
 }
 
 ====================================
 
 //19.get() & put() implementation
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 #include<iostream>
 using namespace std;
 
 int main()
 {
 char ch;
 cout<<"Enter the character\n";
 cin.get(ch);
 cout<<"Entered character:";
 cout.put(ch);
 return 0;
 }
===========================================

//20.character using sequence of get and function
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#include<iostream>
using namespace std;

int main()
{
char ch[3];
cout<<"Enter the character";
cin.get([0]).get([1]).get([2])
cout<<"Entered character was:\n";
cout.put([0]).put([1]).put([2]);
return 0;
}

//21.String get() & put()
~~~~~~~~~~~~~~~~~~~~

#include<iostream>
using namespace std;

int main()
{
 int j=0;
 char x[20];
 cout<<"Enter the string: ";

 while(x[j++]!='\n')
 cin.get(x[j]);

  j=0;

 while(x[j++]!='\n')
 cout.put(x[j]);

 return 0;
}

==================================
//22.Implementation of write() function
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
#include<iostream>
using namespace std;

int main()
{
cout.write("India",6);
cout.write("Is",3);
cout.write("Great",5);
return 0;
}

========================================

//23.Implementation of getline()
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#include<iostream>
#include<string.h>
using namespace std;

int main()
{
 char x[30];
 cout<<"\n Enter any string";
 cin.getline(x,30);
 
 cout<<"\nEntered String is:"<<x; // Method 1
 
 cout<<"\nEntered String is:"; // Method 2
 cout.write(x,30);
 
 cout<<"\nEntered String is:"; //Method 3
 cout.write(x,strlen(x);
 
 return 0;
}
 
 
 ====================================
 
 //25. Using diffirent statement in write()
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 #include<iostream>
#include<string.h>
 using namespace std;
 
 int main()
{
 char a,x[30];
 cout<<"\n Enter the string:";
 cin.getline(x,30);
 cout<<"\n Entered string";
 for(a=0;a<=strlen(x);a++)
 {
   cout<<"\n";
   cout.write(x,a);
 }
 return 0;
 
}

====================================

//26.Use of peek() & ignore()
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#include<iostream>
using namespace std;

int main()
{
 char c;
 cout<<"Enter text";
 while(cin.get(c))
 {
  cout<<c;
  while(cin.peek()=="#")
  {
  cin.ignore(1,'#');
  }
  }
  return 0;
}
========================================



========================================
// 30.To set column width

#include<iostream>
#include<string.h>
using namespace std;

int main()
{
 char ch='b;
 cout.width(5);
 cout<<"A";
 cout.width(15);
 cout<<ch;
 
 return 0;
}

=======================================

//31.both the format of width()
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#include<iostream>
using namespace std;

int main()
{
 cout.width(10);
 cout<<"A";
 int x=cout.width(10);
 cout<<x;
 return 0;
 
}

==============================================
//32.Set precision()
~~~~~~~~~~~~~~~~~~~~
#include<iostream>
using namespace std;

int main()
{
 cout.precision(2);
 cout<<3.1452;
 return 0;
}

=============================================

//33.Display the result of 22/7 in diffirent precision 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#include<iostream>
using namespace std;
  int main()
  {
  int x=0;
  float pi;
  for(x=10;x>=1;x--)
  {
   pi=(float)22/7;
  cout<<precision(x);
  cou<<"\n "<<pi;
  }
  x=cout.precision(1);
  cout<<"\n Previous setting:"<<x;
  return 0;
  }
  
  =====================================
  //34.To fill empty space in a line with a specific symbol(*)
  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
  #include<iostream>
  using namespace std;
  int main()
  {
  cout.fill('*');
  cout.width(10);
  cout<<"H";
  return 0;
  }
  
  ============================================
  
  //35.To fill blank spaces with diffirent symbols
  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
  
  #include<iostream>
  int main()
  {
  cout.fill('/');
  cout.width(20);
  cout<<"WELL"<<endl;
  cout.fill('-');
  cout.width(10);
  cout<<"DONE";
  return 0;
 }
 
 ====================================================
 
 //36.To show the effect cout.fill()
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 #include<iostream>
 using namespace std;
 
 int main()
 {
  cout<<"Begin";
  cout.width(15);
  cout<<"ABC";
  cout<<"\n";
  cout<<"Begin";
  cout.width(15);
  cout.fill('#');
  cout<<"ABC";
  return 0;
}

======================================

//37.To fill the unused filled area with "*"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#include<iostream>
using namespace std;

int main()
{
  int x=0,y=0;
  float pi;
  cout.fill('*');
  for(x=10;x>=1;x--)
  {
    pi=(float)22/7;
    cout.width(j++);
    cout.precision(x);
    cout<<"\n"<<pi;
  }
  
  cout.width(j++);
  cout.precision(x);
  cout<<"\n"<<pi;
  x=cout.fill();
  cout<<"\n Fill setting:"<<(char)x; 
  return 0;
  }
  
  //38.To display the message left and right justified
  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
  
  #include<iostream>
  using namespace std;
  
  int main()
  {
   cout.fill('=');
   cout.setf(ios::right ,ios::adjustfield);
   cout.width(20);
   cout<<"Figure"<<"\n";
   cout.setf(ios::right ,ios::adjustfield);
   cout.width(20);
   cout<<"Figure"<<"\n";
   return 0;
 }
 
 //40.To convert a decimal to hexadecimal
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 #include<iostream>
 using namespace std;
 
 int main()
 {
 cout.setf(ios::hex ,ios::basefield);
 cout<<"\n Hexadecimal of 184 is:"<<184;
 cout.setf(ios::oct , ios::basefield);
 cout<<"\n Octal of 15 is :"<<15;
 cout.setf(ios::dec , ios::basefield);
 cout<<"\n Decimal of 0xfe is:"<<0xfe;
 return 0;
}

//41.Program to use various setting
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#include<iostream>
using namespace std;

int main()
{
 cout.setf(ios::showpos);
 cout<<1254;
 cout.setf(ios::showpoint);
 cout<<"\n"<<1253.524;
 cout.setf(ios::hex,ios::basefield);
 cout<<"\n"<<184;
 cout.setf(ios::uppercase);
 cout<<"\n"<<184;
 return 0;
 }
 
 ==============================
 //42.Display formatted output
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 #include<iotsream>
 #include<iomanip.h>
 using namespace std;
 
 int main()
{
 cout<<setw(10)<<"Hello"<<endl;
 cout<<setw(15)<<setprecision(2) <<2.5555;
 cout<<setiosflags(ios::hex);
 cout<<endl<<"Hexadecimal of 84 is :"<<84;
 return 0;
}

=============================

//To display the given decimal into hexadecimal & octal
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#include<iostream>
#include<iomanip.h>
int main()
{
int a=84;
cout<<"\n Hexadecimal Number:"<<hex<<x;
cout<<"\n Octal Number :"<<oct<<x;
return 0;
}

=====================================================
//45.To demontrate the use of endl
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#include<iostream>
int main()
{
  cout<<"Demo  of endl";
  endl(cout);
  cout<<"It split a line";
  return 0;
  }
 
 =======================================
 //46.Demonstrate the use of flush
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
  #include<iostream>
  using namespace std;
  
  int main()
  {
   char text[20];
   cout<<"Enter text:";
   cin.getline(text,20);
   cout<<"Text Entered"<<text;
   flush(cout);
   return 0;
  }
  
  ================================
  
  //47.create manipulator equivalent to "\t"
  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
  #include<iostream>
  #include<iomanip.h>
  usingnamespace std;
  
  ostream & tab (ostream &o)
  {
   o<<"\t";
   return 0;
  }
  
  int main()
  {
    cout<<1<<tab<<2<<3;
    return 0;
  }
  
  ============================================
  
  

 
 
 
 
 
} 
