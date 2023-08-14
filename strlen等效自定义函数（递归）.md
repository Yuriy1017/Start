# Start
#include <stdio.h>
int my_strlen(char* str)
{
	int count=0;
	while (*str!= '\0')
	{//求字符串长度专用函数
		count++; 
		str++;
    }
	return count;
}
int main()
{
 char arr[]="abc";
 printf(%d",my_strlen)
}
