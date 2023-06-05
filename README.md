# tommy
 #define _CRT_SECURE_NO_WARNINGS = 1;
#include<stdio.h>
#include<math.h>
//int main()
//{
//	int ch = 0;
//	//EOF 文件结束标志 end of file
//	while ((ch = getchar()) != EOF)
//	{
//		putchar(ch);
//	}
//	return 0;
//}
//int main()
//{
//	int ch = 0;
//	while ((ch = getchar()) != EOF)
//	{
//		if (ch < '0' || ch > '9')
//			continue;
//		putchar(ch);
//	}
//
//	return 0;
//}//只输出数字字符
//int main()
//{
//	int i = 0;
//	//初始化 判断 调整
//	for (i = 1; i <= 10; i++)
//	{
//		if (i == 5)
//			break;
//		printf("%d", i);
//	}
//	return 0;
//}
//int main()
//{
//	int a = 0;
//	int b = 0;
//	int c = 0;
//	scanf("%d%d%d", &a, &b, &c);//2 1 3
//	printf("%d %d %d\n", a, b, c);
//	return 0;
//
//}
//int main()
//{
//	int m = 24;
//	int n = 18;
//	int r = 0;
//	scanf("%d%d", &m, &n);
//	while (r=m % n)
//	{
//		m = n;
//		n = r;
//	}
//	printf("%d\n", n);
//		return 0;
//}//取最小公约数
//int main()
//{
//	int year = 0;
//	int count = 0;
//	for (year = 1000; year <= 2000; year++)
//	{
//		////判断year是否为闰年
//		//if (year % 4 == 0 && year % 100 != 0)
//		//{
//		//	printf("%d", year);
//		//	count++;
//		//}
//		//else if (year % 400 == 0)
//		//{
//		//	printf("%d", year);
//		//	count++;
//		//}
//		if (((year % 4 == 0) && (year % 100 != 0)) || (year % 400 == 0))
//		{
//			printf("%d", year);
//			count++;
//		}
//	}
//	printf("\ncount = %d\n", count);
//	return 0;
//}
// 打印素数
int main()
{
	int i = 0;
	int count = 0;
	for(i = 100; i<=200; i++)
	{
		 // 判断i是否为否为素数
		int j = 0;
		for (j = 2; j <=sqrt(i); j++)
		{
			if (i % j == 0)
			{
				break;
			}
		}
		if (j>sqrt(i))
		{
			count++;
			printf("%d", i);
		}
	}
	printf("\ncount = %d\n", count);
	return 0;
}
