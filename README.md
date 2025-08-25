package Car;

public class Car {
	String brand;
	 String model;
	double price;
	double mileage;
	String OwnerName;
	
	static int totalcars;
	static String ShowroomName="NMAMIT";
	
	Car(String brand, String model,double price,double mileage){
		this.brand=brand;
		this.model=model;
		this.price=price;
		this.mileage=mileage;
	    OwnerName="Sanath";
	    totalcars++;    
	}
	Car(String brand, String model,double price,double mileage,String owner)
	{
		this.brand=brand;
		this.model=model;
		this.price=price;
		this.mileage=mileage;
	    this.OwnerName=owner;
	    totalcars++;    
	}
	public String getOwnerName(String owner) {
		return OwnerName;
	}
	public void setOwnerName(String owner) {
		OwnerName=owner;
	}
	public void displayDetails() {
		System.out.println("Brand"+brand);
		System.out.println("Model"+model);
		System.out.println("Price"+price);
		System.out.println("mileage"+mileage);
		System.out.println("owner"+OwnerName);
		}
	public void UpdatePrice(double newPrice) {
		price=newPrice;
	}
	public static void showTotalCars() {
		System.out.println("Total cars"+totalcars);
	}
	public static void showShowroomName() {
		System.out.println("Showroom"+ShowroomName);
		}
}
