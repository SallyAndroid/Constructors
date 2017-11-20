public class World {
	public static void main(String[] args){
		Coder c = new Coder("Bill",59);
		c.describe();
	}
}

public class Coder {
	private String name;
	private int age;
	
	public Coder(String name,int age){
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
