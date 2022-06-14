struct book
{
	char name[20];
	short price;
};
int main()
{
	struct book a1 = { "体验引擎",70 };
	struct book* p = &a1;
	printf("书名=%s\n", (*p).name);
	printf("价格=%d\n", (*p).price);
	a1.price = 60;
		printf("修改后价格=%d\n", (*p).price);
		return 0;
}# -
