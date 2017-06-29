# Trialanguar
Homework1
public class Main {
    public static void main(String[] args) {
        Trialangular trialangular1 = new Trialangular(3.2, 2.2, 4);
        Trialangular trialangular2 = new Trialangular(3, 5 ,7);
        System.out.println(trialangular1);
        System.out.println(trialangular2);
        System.out.println("площадь первого " + trialangular1.area());
        System.out.println("площадь второго " + trialangular2.area());
        }}
        
        
        public class Trialangular {
    private double a;
    private double b;
    private double c;


    public Trialangular(double a, double b, double c) {
        super();
        this.a = a;
        this.b = b;
        this.c = c;
    }
    public Trialangular(){super();}

    public double area(){
        double perimetr = (a+b+c)/2;
        return Math.sqrt(perimetr*(perimetr-a)*(perimetr-b)*(perimetr-c));
    }

    public double getA() {
        return a;
    }

    public void setA(double a) {
        this.a = a;
    }

    public double getB() {
        return b;
    }

    public void setB(double b) {
        this.b = b;
    }

    public double getC() {
        return c;
    }

    public void setC(double c) {
        this.c = c;
    }

    @Override
    public String toString() {
        return "Trialangular{" +
                "a=" + a +
                ", b=" + b +
                ", c=" + c +
                '}';
    }
}

