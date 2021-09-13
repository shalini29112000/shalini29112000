#include <stdio.h>

int main(){
	int N = 0,ans,r;
	scanf("%d", &N);
	
	long data[N];
	for(auto i=0; i<N; i++)
	    scanf("%ld", &data[i]);
	for(auto i=0;i<N;i++)
	{
		r = data[i]%10;
		ans = r*10^N-i-1;
		ans+=r;
	}
	if(ans%10==0)
	printf("Yes");
	else
	printf("No");
    // write your code here
    // ans = 
    //printf("%s", ans);

    return 0;
}
