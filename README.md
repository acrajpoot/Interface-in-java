/*# Interface-in-java*/





interface AtmInterface
{
	int x=4500;
	//public static final int x=4500;
	void deposit();
	//public abstract void deposit();
}
class Sbi implements AtmInterface
{
	Sbi()
	{
		System.out.println("Welcome to Sbi");
	}
	public void deposit()
	{
		int y=7000;
	System.out.println("total amount="+(x+y));
	}
}
class AtmInter
{
	public static void main(String[] args)
	{
	  AtmInterface ai=new Sbi();
      ai.deposit();
	}
}
