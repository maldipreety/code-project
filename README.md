#include <stdio.h>
#include <stdlib.h>
#define SIZE 5
struct stack
{
    int top;
    int data [SIZE];
};
typedef struct stack STACK;
void push (STACK *s,int item)
{
    if (s->top==SIZE-1)
        printf("\n stack over flow");
    else
    {
        s->top=s->top+1;
        s->data[s->top]=item;
    }
}
  void pop(STACK *s)
{
    if (s->top==-1)
        printf("\n stack underflow");
    else
    {
        printf("\n Element pooped is%d",s->data[s->top]);
        s->top=s->top-1;
    }
}
void display(STACK s)
{
    int i;
    if (s.top ==-1)
        printf("\n stack empty");
    else
    {
        printf("\n stack content are\n");
        for (i=s.top; i>0;i--)
            printf("%d\n", s.data[i]);
    }
}

int main()
{
    int ch,item;
    STACK;
    s.top = -1;
    for (;;)
    {
        printf ("\n1 .push");
        printf ("\n2 .pop");
        printf ("\n3 .display");
        printf ("\n4 .exit");
        printf ("\n read choice");
        scanf ("%d", & ch);
        switch (ch)
        {
            case 1:printf("\n read item to be pushed:");
            scanf ("%d", &item);
            push (&s,item);
            break;
            case 2:pop(&s);
            break;
            case 3:display(s);
            break;
            default :exit(0);
        }
    }

    return 0;
}# code-project
code project Description
