#include <iostream>
using namespace std;
class Student 
{
    char name[50]={'\0'};
    string enrollno;
    char  branch[10]={'\0'};
    char clgname[50]={'\0'};
    int a,b,c,d,e,f,g,h,i,j,k,l,m,n,o,p,q,r,s,t;
public:
    void student_details();
    void display_student_details(); // function to show student details
    void rgpv_exam();       // enter data from user
    void test_quiz();       // enter data from user
    void practicals();      // enter data from user
    void midsem();          // enter data from user
    void display_all();
    void average ();
};
void Student ::student_details()
{
    cout << "Enter the name of student :  ";
    cin.ignore();
    cin.getline(name,50);
    cout << endl
         << endl;
    cout << "Enter the enrollment no. of student : ";
    cin >> enrollno;
    cout << endl
         << endl;
    cout << "Enter the Branch of student with stream : ";
    cin.ignore();
    cin.getline(branch,10);
    cout << endl
         << endl;
    cout << "Enter the name of your college : ";
    cin.ignore();
    cin.getline(clgname,50);
    cout << endl
         << endl;
    cout << "***** Student details is succesfully registered *****" << endl;
}
void Student ::display_student_details (){
    cout<<"\n\nName of Student :-               "<<name;
    cout<<"\n\nEnrollment No. of Student :-     "<<enrollno;
    cout<<"\n\nBranch of Student :-             "<<branch;
    cout<<"\n\nName of college :-               "<<clgname;
}
void Student ::rgpv_exam()
{
    cout << "Enter the marks  in rgpv exams out of 70 : " << endl
         << endl;
    cout << "Marks in ARTIFICIAL INTELLIGENCE : ";
    cin >> a;
    cout << "Marks in DATA STRUCTURE  : ";
    cin >> b;
    cout << "Marks in TECHNICAL COMM.  : ";
    cin >> c;
    cout << "Marks in INTRO. TO PROBABILITY AND STATISTICS  : ";
    cin >> d;
    cout << "Marks in OOPM : ";
    cin >> e;     
    cout << endl
         << endl;

    cout << "***** You entered marks is registered in marksheet succesfully ***** " << endl;
}
void Student ::test_quiz()
{
    cout << "Enter the marks in test quiz out of 20 : " << endl
         << endl;
    cout << "Marks in ARTIFICIAL INTELLIGENCE : ";
    cin >> f;
    cout << "Marks in DATA STRUCTURE  : ";
    cin >> g;
    cout << "Marks in TECHNICAL COMM.  : ";
    cin >> h;
    cout << "Marks in INTRO. TO PROBABILITY AND STATISTICS  : ";
    cin >> i;
    cout << "Marks in OOPM : ";
    cin >> j;     
    cout << endl
         << endl;
    cout << "***** You entered marks is registered in marksheet succesfully ***** " << endl;
}
void Student ::practicals()
{
    cout << "Enter the marks of student in practicals out of 30 :  " << endl
         << endl;
    cout << "Marks in ARTIFICIAL INTELLIGENCE : ";
    cin >> k;
    cout << "Marks in DATA STRUCTURE  : ";
    cin >> l;
    cout << "Marks in TECHNICAL COMM.  : ";
    cin >> m;
    cout << "Marks in INTRO. TO PROBABILITY AND STATISTICS  : ";
    cin >> n;
    cout << "Marks in OOPM : ";
    cin >> o;     
    cout << endl
         << endl;
    cout << "***** You entered marks is registered in marksheet succesfully *****" << endl;
}
void Student ::midsem()
{
    cout << "Enter the marks of student in midsem out of 20 : " << endl
         << endl;
    cout << "Marks in ARTIFICIAL INTELLIGENCE : ";
    cin >> p;
    cout << "Marks in DATA STRUCTURE  : ";
    cin >> q;
    cout << "Marks in TECHNICAL COMM.  : ";
    cin >> r;
    cout << "Marks in INTRO. TO PROBABILITY AND STATISTICS  : ";
    cin >> s;
    cout << "Marks in OOPM : ";
    cin >> t;     
    cout << endl
         << endl;
    cout << "***** You entered marks is registered in marksheet succesfully ***** " << endl;
}
void Student :: average (){
    float u = (a+b+c+d+e+f+g+h+i+j+k+l+m+n+o+p+q+r+s+t)/7;
 cout<<"\n\n\n\tThe overall average marks of Student is : "<<u<<"%"<<endl;


   if (u < 100 && u>95){
    cout<<"Student has A+ grade  :"<<endl;
}
          if (u < 95 && u>90){
    cout<<"Student has A grade :"<<endl;
}
      if (u < 90 && u>80){
    cout<<"Student has B+ grade  :"<<endl;
}
       if (u < 80 && u>70){
    cout<<"Student has B grade :"<<endl;
}
       if (u < 70 && u>60){
    cout<<"Student has C+ grade  :"<<endl;
}
       if (u < 60 && u>55){
    cout<<"Student has C grade  :"<<endl;
}     
       if (u < 60 && u>40){
    cout<<"Student has B grade :"<<endl;
}   
     if (u<40){
        cout<<"You are fail : "<<endl;
     }
}
void Student ::display_all()
{
  cout<<"\n\n\n\t RAGIV GANDHI PROUDYOGIKI VISHWAVIDHYALAYA (BHOPAL)  " ;
  this->display_student_details();
  cout<<"\n\n";
  cout<<"S.no.   SUBJECTS                             RGPV EXAM   MID SEM   PRACTICALS   TEST QUIZ  \n\n";
  cout<<"01."<<"  AARTIFICIAL INTELLIGENCE                  "<<a<<"           "<<p<<"            "<<k<<"       "<<f <<endl;
  cout<<"02."<<"  DATA STRUCTURE                            "<<b<<"           "<<q<<"            "<<l<<"       "<<g<<endl;
  cout<<"03."<<"  TECHNICAL COMM.                           "<<c<<"           "<<r<<"            "<<m<<"       "<<h<<endl;
  cout<<"04."<<"  INTRO. TO PRO. AND STATISTICS             "<<d<<"           "<<s<<"            "<<n<<"       "<<i<<endl;
  cout<<"05."<<"  OOPM                                      "<<e<<"           "<<t<<"            "<<o<<"       "<<j<<endl;
 this->average();
}
int main()
{
    Student s1;
          cout<<"\t******** WELCOME TO THE STUDENT ACADEMIC PERFORMENCE SHEET ********";
         cout<<"\n\n\n\tIF YOU WANT TO SEE STUDENT ACADEMIC PERFORMENCE FOLLOW THE SOME STEPS ";
         cout<<"\n\n### Enter student details ### \n\n";
         s1.student_details ();
         cout<<"\n\n ### Enter rgpv exam marks ###\n\n ";
         s1.rgpv_exam();
         cout<<"\n\n ### Enter practical marks ###\n\n";
         s1.practicals ();
         cout<<"\n\n ### Enter midsem marks ###\n\n ";
         s1.midsem();
         cout<<"\n\n ### Enter test quiz marks ### \n\n";
         s1.test_quiz();
         cout<<"\n\n### student academic performence sheet ### ";
         s1.display_all();
         cout<<"\n\n\n***** Thanks for using this platform *****";
    return 0;
}
