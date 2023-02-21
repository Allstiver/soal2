// soal2
#include <iostream>
using namespace std;

int main()
{
    int matrix[3][3];
    int determinan;

    
    cout << "enter number of determinan 3*3 :" << endl;
    for (int i = 0; i < 3; i++)
    {
        for (int j = 0; j < 3; j++)
        {
            cin >> matrix[i][j];
        }
    }

  
    determinan = (matrix[0][0] * ((matrix[1][1] * matrix[2][2]) - (matrix[1][2] * matrix[2][1]))) - (matrix[0][1] * ((matrix[1][0] * matrix[2][2]) - (matrix[1][2] * matrix[2][0]))) + (matrix[0][2] * ((matrix[1][0] * matrix[2][1]) - (matrix[1][1] * matrix[2][0])));

   
    cout << "determinan barabar ast ba : " << determinan << endl;

    return 0;
}
