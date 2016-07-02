# removedup
#include <stdio.h>
#include<string.h>
int main(void) 
{
	char string[50];
	int array[26]={0},len,i;
	scanf("%s",string);
	len=strlen(string);
	for(i=0;i<len;i++)
		array[string[i]-'a']++;
	for(i=0;i<len;i++)
	{
			if(array[string[i]-'a']>1)
			{
				printf("%c",string[i]);
				hash[string[i]-'a']=0;
			}
	}
	return 0;
}
