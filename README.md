# inheritence-program

package shape.inheritence.examples;
abstract class Shape{
    public abstract double calculateArea();
    

}
class Circle extends Shape{
  private double radius;
public Circle(double radius){
    this.radius = radius;
}  
@Override
public double calculateArea(){
    return Math.PI*radius*radius;
   
}
}
class Rectangle extends Shape{
    private double length, width;
    public Rectangle(double length, double width){
        this.length= length;
        this.width= width;
        
    }
 @Override
 public double calculateArea(){
     return length* width;
 }
}
class Square extends Shape{
    private double side;
    public Square(double size){
        this.side= side;
  
   }

@Override
public double  calculateArea(){
return side*side;

}
}
class Triangle extends Shape{
    private double base,height;
    public Triangle(double base, double height){
        this.base= base;
        this.height= height;
        
    }

@Override
public double calculateArea(){
return 0.5*base*height;
}
}
/**
 *
 * @author 1BSCCSA43
 */
public class ShapeInheritenceExamples {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
       // TODO code application logic here
    Shape circle = new Circle(5);
    Shape rectangle= new Rectangle(4,6);
    Shape square = new Square(4);
    Shape triangle = new Triangle(3,5);
    
        System.out.println("Circle Area:" + circle.calculateArea());
        System.out.println("Rectangle Area:" + rectangle.calculateArea());
        System.out.println("Square Area:" + square.calculateArea());
        System.out.println("Triangle Area:" + triangle.calculateArea());
    } 
}


outut ;
Circle Area:78.53981633974483
Rectangle Area:24.0
Square Area:0.0
Triangle Area:7.5
BUILD SUCCESSFUL (total time: 0 seconds)

