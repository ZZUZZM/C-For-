# C-For-
//将一个二维数组行和列元素互换，存到另一个二维数组中
#include <iostream>
using namespace std;
int main()
{
	int a[2][3] = { { 1, 2, 3 }, { 4, 5, 6 } };
	int b[3][2], i, j;
	cout << "array a:" << endl;
	for (i = 0; i <=1; i++)// 两行
	{
		for (j = 0; j <= 2; j++)//三列
		{ 
			cout << a[i][j] << " ";
			b[j][i] = a[i][j];//行列元素交换
		}
		cout << endl;
	}
	cout << "array b:" << endl;
	for ( i = 0; i <= 2; i++)
	{
		for (j = 0; j <= 1; j++)
			cout << b[j][i] << " ";
	cout << endl;
	}
	return 0;
}
