# Aleksandra Vorobyova
## Contacts  

Telephone:  +375296820335;

Gmail:  aleksa1601@gmail.com;

Address:  2201140 Timoshenko street, 12-82, Minsk, Belarus.  

## Summary

* Excellent communication (verbal and written) and interpersonal skills; able to communicate effectively to management, users, developers and cross-functional team members;
* Well-developed analytical and problem solving skills.  

## Skills

* Basic knowledge of *C++, PHP, JavaScript, HTML, CSS*;
* Proficient in *Microsoft Office* including Excel and Powerpoint;
* *Google Drive, GitHub*.

### *C++ code example*

    #include <iostream>
    #include <iomanip>
    #include <cmath>
    using namespace std;

    int main ()
    {
        const int n=4;
        double mas[n][n]= {
            {9,-2,-5,1},
            {2,9,1,5},
            {1,2,11,-4},
            {1,-1,-4,10}
            };
        double B[n]={3,-3,-3,22};
        int i = 0;
        double s;
        int preobl=0;
        int preobll=0;
        int sum[i];
        double L[n][n]={0};
        double U[n][n]={0};
    
        for(i=0;i<n;i++)
        {
            for(int j=0;j<n;j++)
            { if(i!=j)
            {
                sum[i]+= abs(mas[i][j]);
            }
            }
        }
        cout << "Proverim na diagonalnoe preobladanie:"<<endl;
        for (i=0;i<n;i++)
        
        {
        
            cout <<"sum [" << i << "]="<< sum[i]<< endl;
        
        }
    
        for (i = 0; i < n; i++){
            if (abs(mas[i][i]) < sum[i])
            {preobl=1;break;}}
    
        for (i = 0; i < n; i++){
            if (abs(mas[i][i]) == sum[i])
            {preobll++; }}
    
        if (preobll==4) {preobl=1;}
        if (preobl ==1) {cout << "Diagonalnoe preobladanie net"<<endl;
            return 0;}
        else {cout << "Diagonalnoe preobladanie est"<< endl;
        
            for (int i = 0; i < n; i++)
            {
                for (int j = 0; j < n; j++)
                {
                    if (i == j)
                    {L [i][j] = 1;}
                }
            }
            for (int i = 0; i < n; i++)
            {
            
                for (int j = 0; j < n; j++)
                {
                    if (i <= j)
                    {
                    
                        s = 0;
                        for (int k = 0; k < i; k++)
                        {s += L [i][k] * U [k][j];}
                        U [i][j] = mas [i][j] - s;
                        }
                    else
                    {
                        for (int z=i; z < n; z++)
                        {
                            s = 0;
                            for (int k = 0; k < j; k++)
                            {s += L [z][k] * U [k][j];}
                            L [z][j] = (mas [z][j] - s)/U[j][j];
                        }
                    }
                
                }
            
            }
        
            cout << "\nMatriza L:\n";
            for (int i = 0; i < n; i++)
            {
                for (int j = 0; j < n; j++)
                    cout << " " << L [i][j] << " ";
                    cout << «\n\n»;
            }
        
            cout << "\nMatriza U:\n";
        
            for (int i = 0; i < n; i++)
            {
                for (int j = 0; j < n; j++)
                cout << " " << U [i][j] << " ";
                cout << "\n\n";
            }
            cout << "Reshaem, ispolzya LU-razlozenie:"<< endl;
            double y[n]={0};
            for (int i = 0; i < n; i++)
            {
                double s1 = 0;
                for (int k = 0; k < i ; k++)
            {
                s1 += L[i][k] * y[k];
            }
            y[i] = B[i] - s1;
            }
            cout << "Matriza Y:" << endl;
            for (int i=0; i<n; i++)
            {
            cout <<" Y["<< i+1 << "]=" <<y[i];
            cout << endl;
             }
            cout << endl;
        
            double x[n]={0};
            for (int i = n-1 ; i >= 0; i--)
            {
                double s3 = 0;
                for (int k = n-1 ; k >=0; k--)
            {
                s3 += U[i][k] * x[k];
            }
                x[i] = (y[i] - s3)/(U[i][i]);
            }
        
            cout << "Matriza X (reshenie) :" << endl;
            for (int i=0; i<4; i++)
            {
            cout <<" X["<< i+1 << "]=" <<x[i];
            cout << endl;
            }
            cout << endl;
            double det=1;
            for (int i=0;i<4;i++)
            {
                det*=U[i][i];
            }
            cout <<" Opredelitel = "<< det;
        }
        return 0;
    }

## Experience

Yves Rocher Group (3-month in 2018)

Achievements and Contributions:
1. Customer Service: Responded to incoming calls. Screened telemarketing and direct sales orders.
2. Administration: Ensured to supervisor for approval.
3. Records Processing: Entered customer information into internal records management system. 

## Education

Belarus State Economic University  
Faculty of Economics and Management  
Pending Bachelor’s degree(Expected June 2021)

## English Level

*Upper-Intermediate level*  
Has completed a 144-hour general English Course in a Streamline language school.