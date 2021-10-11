#include <iostream>
using namespace std;

int del(int numbers)
{
int sum = 0;
for (int i = 1; i <= (numbers / 2); i++)
{
if (numbers % i == 0)
{
sum += i;
}
}

return sum;
}

int main()
{

for (int i = 2; i <= 10000; i++)
{
if (i == del(del(i)))
{
cout « i « " " « del(i) « endl;
}
}

system("pause");
return 0;
}
