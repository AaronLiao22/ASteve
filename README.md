# ASteve
Student

public class Main {
	
	public static void main(String[] args) {
		Person a = new Person("Julius");
		Person b = new Person("James");
		a.setAge(123);
		a.setAddress("ww");
		b.setAge(1234);
		b.setAddress("xx");
		System.out.println(a.getName());
		System.out.println(a.getAge());
		System.out.println(a.getAddress());
		System.out.println(b.getName());
		System.out.println(b.getAge());
		System.out.println(b.getAddress());
		a.greet(b);
	}
}		

----------------------------------------------------------
public class Person {
	private String name = null;
	private int age = 0;
	private String address = null;
	
	public Person(String name) {
		this.name = name;
	}
	public String getAddress() {
		return this.address;
	}
	public String getName() {
		return this.name;
	}
	public int getAge() {
		return this.age;
	}
	public void setAddress(String address) {
		this.address = address;
	}
	public void setName(String name) {
		this.name = name;
	}
	public void setAge(int age) {
		this.age = age;
	}
	public void greet(Person p){
		System.out.println("Hi " + p.getName() + " My name is " + this.name);
	}

}
