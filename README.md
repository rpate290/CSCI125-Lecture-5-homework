# CSCI125-Lecture-5-homework
package lecture5Hw;

interface MessageEncoder{
abstract void encode(String plainText, int shift);
}

public class SubstitutionCipher implements MessageEncoder {
	int shift;
	SubstitutionCipher(int s){
		shift=s;}
	 public void encode(String plainText, int shift) {
		char[] messageArray= plainText.toCharArray();
		for (char i: messageArray) {
			i+=shift;
			System.out.print(i);}}
		public static void main(String[] args) {
			int shift= 1;
			String message= "hello";
			System.out.println(message);
			MessageEncoder p= new SubstitutionCipher(shift);
			p.encode(message, shift);
		}
	

	}
