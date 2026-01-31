- 👋 Hi, I’m @Soofmax
- 👀 I’m interested in Githubproject.
- 🌱 I’m currently learning .
- 💞️ I’m looking to wellou thing.
- 😄 Call me Soo , Soofmax or just S.
- ⚡ Go to the funny world .;)

<!---
Soofmax/Soofmax is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
void    ft_putchar(char c);

void    print_line(int x, char left, char mid, char right)
{
    int    i;

    if (x <= 0)
        return ;
    ft_putchar(left);
    i = 1;
    while (i < x - 1)
    {
        ft_putchar(mid);
        i++;
    }
    if (x > 1)
        ft_putchar(right);
    ft_putchar('\n');
}

void    rush(int x, int y)
{
    int    j;

    if (x <= 0 || y <= 0)
        return ;
    print_line(x, 'o', '-', 'o');
    j = 1;
    while (j < y - 1)
    {
        print_line(x, '|', ' ', '|');
        j++;
    }
    if (y > 1)
        print_line(x, 'o', '-', 'o');
}