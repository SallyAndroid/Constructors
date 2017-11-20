public class World {
	public static void main(String[] args){
		Coder c = new Coder();
		c.describe();//int的默认值是0.一个空的对象引用变量（指向一个对象的一个变量）的默认值是null。
	}
}

public class Coder {
	private String name;
	private int age;
	
	public void initialize(String name,int age){
		this.name = name;
		this.age = age;
	}
	
	public void weiteCode(){
		System.out.println(name + " is coding!");
	}
	
	public void describe(){
		System.out.println("I am a coder");
		System.out.println("My name is " + name);
		System.out.println("I am " + age +" years old");
	}
}
