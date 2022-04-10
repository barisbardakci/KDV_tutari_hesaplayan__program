# KDV_tutari_hesaplayan__program

Ödev
Eğer girilen tutar 0 ve 1000 TL arasında ise KDV oranı %18 , tutar 1000 TL'den büyük ise KDV oranını %8 olarak KDV tutarı hesaplayan programı yazınız.

KDV'yi ürünün fiyatına göre atar ve KDV tutarı ve KDV dahil tutarını gösterir.
import java.util.Scanner;
public class Main{
	public static void main(String[] args) {
		float kdvHaric, kdvTutari, kdvDahil ;
		Scanner kdv=new Scanner(System.in);
		System.out.println("KDV hariç tutar : ");
		kdvHaric=kdv.nextFloat();
		
		int kdvOranı= kdvHaric <= 1000? 18:8 ;
		kdvTutari=kdvHaric*kdvOranı/100 ;
		kdvDahil=kdvHaric+kdvTutari ;
		
		System.out.println("KDV tutarı : " + kdvTutari);
		System.out.println("KDV dahil tutar :" + kdvDahil);
		
	}
}
