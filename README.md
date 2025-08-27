# design-of-a-bill-in-c-
made a bill design in c++


#include<iostream>
#include<stdlib.h>
#include<stdio.h>

using namespace std;

int main(){
	char med[5][20];
	int i,m[5],c[5],msum,tsum;
	msum=0;
	tsum=0;
	for(i=0;i<5;i++){
		cout<<"Medicine=";
		gets(med[i]);
		fflush(stdin);
		cout<<"Enter no of medicine=";
		cin>>m[i];
		cout<<"Enter cost of one medicine=";
		cin>>c[i];
	}
	system("clear");
	cout<<"____________________________________________________________________________";
	cout<<endl;
	cout<<"|";
	cout.width(15);
	cout<<"Medicines";
	cout.width(5);
	cout<<"|";
	cout.width(15);
	cout<<"no of meds";
	cout.width(5);
	cout<<"|";
	cout.width(18);
	cout<<"cost of 1 med";
	cout.width(5);
	cout<<"|" ;
	cout.width(11);
	cout<<"Total cost";
	cout.width(2);
	cout<<"|"<<endl;
	cout<<"------------------------------------------------------------------------------";
	cout<<endl;
	for(i=0;i<5;i++){
		cout<<"|";
		cout.width(15);
		cout<<med[i];
		cout.width(5);
		cout<<"|";
		cout.width(15);
		cout<<m[i];
		cout.width(5);
		cout<<"|";
		cout.width(18);
		cout<<c[i];
		cout.width(5);
		cout<<"|" ;
		cout.width(11);
		int k=m[i]*c[i];
		cout<<k;
		cout.width(2);
		cout<<"|"<<endl;
		tsum=tsum+k;
		msum=msum+m[i];
	}
	cout<<"|";
	cout.width(20);
	cout<<"|";
	cout.width(15);
	cout<<msum;
	cout.width(5);
	cout<<"|";
	cout.width(23);
	cout<<"|";
	cout.width(11);
	cout<<tsum;
	cout.width(2);
	cout<<"|";
	cout<<endl;
	cout<<"|___________________________________________________________________________|";
	return 0;
}
