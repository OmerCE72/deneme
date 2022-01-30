kpog tam sayı dizisinin her bir satırın toplamını geri döndüren programı yapınız 

package ömer;
import java.util.Scanner;
public class örn6 {
public static String ikidizi(int [][]a) {
	int top=0;
	int enb=a[0][0];
	for(int i=0;i<a.length;i++) {
		top=0;
		for(int j=0;j<a.length;j++) {
			top+=a[i][j];
		}
		System.out.println((i+1)+".satırın toplamı : " + top);
	}
	return ""  ;
}
	public static void main(String[] args) {
		int [][] a=new int[2][2];
		Scanner k=new Scanner(System.in);
		for(int i=0;i<a.length;i++) {
			for(int j=0;j<a.length;j++) {
			a[i][j]=k.nextInt();
			}
		}
	   
		System.out.println(ikidizi(a));
	}
}
