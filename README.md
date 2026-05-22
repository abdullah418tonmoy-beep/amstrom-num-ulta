#include<stdio.h>
#include<math.h>
int main()
{
    int num, result = 0, orginal, reminder,n=0;

    printf(" ENTER YOUR NUMBER: ");
    scanf("%d", &num);

    orginal = num;

    while (orginal != 0)
    {
        orginal /= 10;
        n++;

    }

    orginal = num;
       while(orginal != 0)
       {
           reminder=orginal%10;
           result= result+pow(reminder,n);
            orginal /= 10;
       }

       if (result==num)
    {
        printf(" %d is amstronm", num);
    }

    else
         {
        printf(" %d is not amstronm", num);
    }

    return 0;
}
