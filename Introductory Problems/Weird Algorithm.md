```
#include <iostream>

using namespace std;

long long int compute(long long int N)
{
	if(N == 1) return N;

	while(N != 1)
	{
		cout << N << " ";
		N = N%2 == 0 ? N/2 : N*3 + 1;
	}
	return 1;
}

int main()
{
	long long int N; cin >> N;
	cout << compute(N);

	return 0;
}
```
