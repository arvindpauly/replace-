# replace-
import java.util.Scanner;

public class Remove {
	public static void main(String[] args) {
		Scanner a = new Scanner(System.in);
		System.out.println("enter  the String");
		String s1 = a.next();
		char[] array = s1.toCharArray();
		char[] arr = new char[s1.length()];
		int k = 0;
		int count = 0;
		for (int i = 0; i < array.length; i++) {
			for (int j = 0; j <= i; j++) {
				if (array[i] == arr[j]) {
					count++;
					continue;
				}

			}
			if (count == 0)
				arr[k++] = (array[i]);
			count = 0;

		}
		for (int g : arr) {
			System.out.print((char) g);
		}

	}
}
