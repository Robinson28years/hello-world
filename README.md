# hello-world
#include <stdio.h>
#include <math.h>
#include <string.h>
int main()
{
	int pos=-1,man[1000]={0},t=0,count=0,num;
	scanf("%d",&num);
	while(1)
	{
		pos=(pos+1)%num;
		if(man[pos]==0)
		{
			//printf("OK\n");
			
			t++;
			//printf("%d\n",t);
			
			if(t==5)
		{
			//printf("OK2\n");
			count++;
			man[pos]=count;
			//printf("%d  %d\n",pos,count);
			
			t=0;
		}
		}
		
		//pos++;
		if(count==num)
		{
			printf("%d\n",pos+1);
			break;
		}
	}
	return 0;
}
