# 33.-Runtime-polymorphism-

class Vehicle {
    public void start() {
        System.out.println("Vehicle is starting");
    }
}
class Car extends Vehicle {
    @Override
    public void start() {
        System.out.println("Car is starting with key");
    }
}
class Motorcycle extends Vehicle {
    @Override
    public void start() {
        System.out.println("Motorcylce is starting with a kick");
        
    }
}


public class VehicleTest {

        public static void main(String[] args) {
        
        Vehicle v1 = new Vehicle();
        Vehicle v2 = new Car();
        Vehicle v3 = new Motorcycle ();
        
        v1.start();
        v2.start();
        v3.start();
    }
    
}

Output

run:
Vehicle is starting
Car is starting with key
Motorcylce is starting with a kick
