# Hackerearth-Data-Structures-Problems
/*Micro and Array Update
Micro purchased an array A having N integer values. After playing it for a while, he got bored of it and decided to update value of its element. In one second he can increase value of each array element by 1. He wants each array element's value to become greater than or equal to K. Please help Micro to find out the minimum amount of time it will take, for him to do so.

Input: 
First line consists of a single integer, T, denoting the number of test cases. 
First line of each test case consists of two space separated integers denoting N and K. 
Second line of each test case consists of N space separated integers denoting the array A.

Output:
For each test case, print the minimum time in which all array elements will become greater than or equal to K. Print a new line after each test case.*/

 #include<stdio.h>
void main()
{
    int t;
    int i,j,k,n;
    scanf("%d",&t);
    for(i=0;i<t;i++)
    {
        scanf("%d %d",&n,&k);
        int min=k;
        int a[n];
        for(j=0;j<n;j++)
        {
            scanf("%d",&a[j]);
            if(a[j]<min)
                min=a[j];
        }
        printf("%d\n",k-min);
    }
}
