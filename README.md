
1

class Number1{
private int n1;
private int n2;
Number1(int n1,int n2){
this.n1=n1;
this.n2=n2;
}
public void addition(){
p(n1+n2);}
public void subtration(){
p(n1-n2);}
public void multiplication(){
p(n1*n2)}
public void division(){
p(n1/n2);}
public void p(int n){
System.out.println(n);}
}
class Number2{
public static void main(string[]  args){
Number1=new Number();
n.addtion();
n.subtration();
n.multiplication();
n.division();
}
}


2


public class Person{
private String name;
private int age;
public Person(String name,int age){
this.name=name;
this.age=age;}
public void display(){
System.out.println("姓名: "+this.name+"\n年龄: "+this.age);
}
public class Textperson {
public static void main(string[]  args){
Person person=new Person();
person.display();
}
}







3





public class GetSet {
    String name;
    GetSet(String name){
        this.name = name;
    }
    GetSet(){
 
    }
    public void setName(String name){
        this.name = name;
    }
    public String getName(){
        return this.name;
    }
 
    public static void main(String[] args) {
        GetSet per = new GetSet("杨洋");
        System.out.println(per.getName());
        per.setName("黄渤");
        System.out.println(per.getName());
 }





4




public class TestWuMingFen{
    public static void main(String []args){
        WuMingFen f1 = new WuMingFen("牛肉",3,true);
        WuMingFen f2 = new WuMingFen("牛肉",2);
        WuMingFen f3 = new WuMingFen();

        f1.check();
        f2.check();
        f3.check();
    }
}

class WuMingFen{
    private String theMa;
    private int quantity;
    private boolean likeSoup;
    private boolean refer = false;

    public WuMingFen(String theMa, int quantity){
        this.theMa = theMa;
        this.quantity = quantity;
        refer = true;
    }
    public WuMingFen(String theMa, int quantity, boolean likeSoup){
        this.theMa = theMa;
        this.quantity = quantity;
        this.likeSoup = likeSoup;
    }
    public WuMingFen(){
        this.theMa = "酸辣粉";
        this.quantity = 2;
        this.likeSoup = true;
    }

    public void check(){
        System.out.println("面    码: " + this.theMa);
        System.out.println("粉的分量: " + this.quantity + "两");
        if(!this.refer){
    System.out.println("是否带汤: " + ((this.likeSoup == true)? "带汤" : "不带汤"));
        }else{
            System.out.println("是否带汤: 未知");
        }
        System.out.println();
    }
    }







5



public class Vehicles {
    static String brand;
    static String color;

    private static void run() {
        System.out.println("我已经开动了");

    }
    private static void init() {
        Vehicles vehicles = new Vehicles();
        vehicles.setBrand("宝马");
        vehicles.setColor("白色");
        Car car = new Car();
car.setSeats(15);
Truck truck = new Truck();
truck.setLoad(20);
    }
    public static class Truck extends Vehicles{
        static float load;

        public float getLoad() {
        return load;
        }
        public void setLoad(float load) {
            this.load = load;
        }
    }
    public static class Car extends Vehicles{
        static int seats;

        public int getSeats() {
            return seats;
        }
        public void setSeats(int seats) {
            this.seats = seats;
        }
}
public static void main(String[] args) {
        init();
        run();
        showInforclk();
        showCar();
        showTruck();
        System.out.println(brand);
        System.out.println(color);
        System.out.println(Car.seats);
        System.out.println(Truck.load);
    }
    private static void showTruck() {
    }

    private static void showCar() {
    }
     public String getBrand() {
        return brand;
    }

    public void setBrand(String brand) {
        this.brand = brand;
    }

    public String getColor() {
        return color;
    }

    public void setColor(String color) {
        this.color = color;
    }

    private static void showInforclk() {
    }
}








6


public class NetWeb {
    static int id;
    static int password;
    static String email;

    public static void main(String[] args) {
       NetWeb netWeb = new NetWeb();
      netWeb.setId();
      netWeb.setPassword();
      netWeb.setEmail(email);
        System.out.println(NetWeb.id);
        System.out.println(NetWeb.password);
        System.out.println(NetWeb.getEmail());
       }
    public NetWeb() {
    }
    public NetWeb(int id, int password, String email) {
        this.id = id;
        this.password = password;
        this.email = email;
    }
    public int getId(){
    return id;}
    public void setId(int id){
    this.id=id;}
    public int getPassword(){
    return password;}
    public void setPassword(int password){
    this.password=password;}
    public string getEmail(){
    return email=id+"@gameschool.com";}
    public void setEmail(string email){
    this.email=email;}
    public String toString() {
    return "NetWeb{id = " + id + ", password = " + password + ", email = " + email + "}";
    }
    } 







10

public class StaticDemo {
    public static int num=10;
    public int num1=5;
    public static void main(String[] args) {
        System.out.println("num="+StaticDemo.num);
        StaticDemo staticDemo = new StaticDemo();
        System.out.println("num1="+staticDemo.num1);
    }
}



9


public class Number{
public Number1(int a,int b){
if(a>b)
System.out.println(a);
else
System.out.println(b);
}
public Number2(double a,double b,double c){
System.out.println(a*b*c);
}
public Number3(String s1,String s2){
if(s1.equals(s2))
System.out.println("equal");
else
System.out.println("no equal");
}
public static void main(String[] args)
{
new Number1(1,2);
new Number2(3.3,1.0,2.8);
new Number3("welcome","beijing");
}
}



8


public class Car {
    private int TiresNum;
    private String color;
    private double weight;
    private int speed;
    public Car() {
    }
    public Car(int tiresNum, String color, double weight) {
        this.TiresNum = tiresNum;
        this.color = color;
        this.weight = weight;
    }
    public void speedUp(int speed){
        System.out.println("加速"+speed+"km/s");
        this.speed+=speed;
    }
    public void speedDown(int speed){
        System.out.println("减速"+speed+"km/s");
        this.speed-=speed;
    }
    public void stop(){
       speed=0;
        System.out.println("停车");
    }
    public int getTiresNum() {
        return TiresNum;
    }
    public void setTiresNum(int tiresNum) {
        TiresNum = tiresNum;
    }
    public String getColor() {
        return color;
    }
    public void setColor(String color) {
        this.color = color;
    }
    public double getWeight() {
        return weight;
    }
    public void setWeight(double weight) {
        this.weight = weight;
    }
    public int getSpeed() {
        return speed;
    }
    public void setSpeed(int speed) {
        this.speed = speed;
    }
    public String toString() {
        return  "轮胎数=" + TiresNum +"个", "颜色" color + '\'+"重量" + weight +"kg"," 速度
" speed+"km/s";
    }
}
class CarTest{
    public static void main(String[] args) {
        Car car = new Car();
        car.setTiresNum(8);
        car.setColor("biase");
        car.setWeight(600.5);
        System.out.println(car.toString());
        car.carStatus();
        car.stop(0);
        car.carStatus();
        car.speedUp(80);
        car.carStatus();
        car.speedDown(30);
        car.carStatus();
}























































# java
