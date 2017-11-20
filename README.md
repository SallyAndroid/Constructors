public class World {
	public static void main(String[] args){
		Coder c = new Coder("Bill",59);
		c.describe();
		System.out.println("");
		
		String cName = c.getName();
		int cAge = c.getAge();
		
		System.out.println(cName + "," + cAge);
		System.out.println("");
		c.setName("Steve");
		c.setAge(-5);
		
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
	public String getName(){
		return name;
	}
	
	public int getAge(){
		return age;
	}
	
	public void setName(String newName){
		if(newName != null){
			name = newName;
		}else{
			System.out.println("Invalid name provided!");
		}
	}
	
	public void setAge(int newAge){
		if(newAge > 0){
			age = newAge;
		}else{
			System.out.println("Invalid age provided");
		}
	}
	
}
