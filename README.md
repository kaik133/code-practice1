/占いゲーム/
public class Main { 
  public static void main(String[] args) {
    System.out.println("ようこそ占いの館へ");
    System.out.print("あなたの名前を入力してください＞");
    String name = new java.util.Scanner(System.in).nextLine(); //キーボードからの”名前”入力の受付
    System.out.print("あなたの年齢を入力してください＞");
    String ageString = new java.util.Scanner(System.in).nextLine(); //キーボードからの"年齢"入力の受付
    int age = Integer.parseInt(ageString);
    int fortune = new java.util.Random().nextInt(4);
    fortune++;
    System.out.println("占いの結果が出ました！");
    System.out.println(age + "歳の" + name + "さん、あなたの運気番号は" + fortune + "です");
    System.out.println("1: 大吉　2:中吉　3:吉　4: 凶");
 }
}
