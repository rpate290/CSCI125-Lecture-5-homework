# CSCI125-Lecture-5-homework
package lecture5Hw;

public class Hw5 {

abstract class payCalculator{
	double computePay(double pay, double hours) {
		return hours*pay;
	}
class regularPay extends payCalculator{
	regularPay(double i,double n){
		 double payRate= i;
	     double hours= n;
		
	}

	
}
class hazardPay extends payCalculator{
	double computePay(double pay, double hours) {
		return hours*pay*1.5;
	}
abstract class discountPolicy{
	double itemCount;
	double itemCost;
	abstract double computeDiscount(double count, double itemcost);
class bulkDiscount extends discountPolicy{
	int minimum;
	double discount;
	double total;
	bulkDiscount(int m, double p){
	minimum=m;
	discount=p;}
	double computeDiscount(double count,  double itemcost) {
		if(count>minimum){
		double total=itemcost/2;
		return total;}
		else {
		double total=itemcost;
		return total;
			
		}
		
	}
	
		 
}}
	public static void main(String[] args) {
		// TODO Auto-generated method stub

	}

}}}
