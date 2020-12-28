# H.W21.12.2020

1 . מה ההבדל בין int ל-float?
תשובה:
Int למספרים שלמים.
Float למספרים עשרוניים.

2. מהו ? Scanne 
תשובה:
קליטה מהמשתמש\מקלדת

3. מה עושה הפקודה System.out.println() ?
תשובה:
מדפיסה למשתמש פלט, הפלט הרצוי נכתב בתוך הסוגריים.

package com.company;

import java.util.Random;
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
    

        //4 .צור משתנה int ותן לו את הערך 5 .צור משתנה נוסף עם הערך 12 + 20 .
        //צור משתנה float עם הערך 5.7 .

        int number = 5;
        int number2 = 12 + 20;

        float num = 5.7f;

        //5 .צור שני משתנים מסוג int :a ו-b .לאחר מכן צור משתנה בשם sum שהערך שלו הוא הסכום של a ו-b .צור
        //משתנה בשם multiply שהערך שלו הוא המכפלה של a ו-b .
        // כאן בשאלה אין התייחסות למה יהיה בתוך המשתנים, אז זה פחות קריטיץ רוצים לראות שאת יודעת לעשות חיבור וכפל תודה

        int a = 1;
        int b = 1;
        int sum = a + b;
        int multiply = a * b;

        //6 .צור מחרוזת )String )בשם color ובה הכנס את הצבע האהוב עליך.

        String color = "pink";

        //7 .צור מחרוזת בשם name וקלוט לתוכה את השם מן המשתמש.
        //לאחר מכן הדפס ברכה למשתמש: "!Java to Welcome, X Hello( "כאשר X הוא שם המשתמש שהוכנס(.
        Scanner s = new Scanner(System.in);
        System.out.println("pleas enter your name");
        String name = s.nextLine();
        System.out.println("hello" + " " + (name) + " " + "welcome to java");

        //8 .צור משתנה int בשם year והכנס לו את הערך 2020 .כעת הוסף לו 10 ,ולאחר מכן הפחת ממנו 30( עשה
        //זאת בפורמט מקוצר(. לבסוף הדפס את המשתנה. מה קיבלת?
        int year = 2020;
        year += 10;
        year -= 30;
        System.out.println(year);

        //9 .קלוט שלושה מספרים והדפס את הממוצע שלהם. )רמז: חשב את הממוצע כך - סכום המספרים חלקי 3
        System.out.println("Please enter 3 numbers:");
        int x = s.nextInt();
        int y = s.nextInt();
        int z = s.nextInt();
        System.out.println("The memuza is " + (x + y + z) / 3f);

        //10. קלוט מהמשתמש מספר )מהירות נסיעה( לתוך משתנה int בשם speed .
        //אם המהירות גדולה מ-120 - הדפס " !fast too "
        //אם המהירות קטנה מ-80 - הדפס " !slow too "
        //בכל מקרה אחר, הדפס " driver good "
        {
            System.out.println("pleas enter namber");
            int speed = s.nextInt();
            if (speed >= 120) {
                System.out.println("fast too!");
            } else if (number <= 80) {
                System.out.println("slow too!");
            } else
                System.out.println("driver good");


            // Question number 11 from the targil

            System.out.println("Please enter tomer's age");
            int tomerAge = s.nextInt();
            System.out.println("Please enter dany's age");
            int danyAge = s.nextInt();

            if (tomerAge == danyAge) {
                System.out.println("Same age");
            } else if (tomerAge > danyAge) {
                System.out.println("Tomer is older");
            } else {
                System.out.println("Dany is older");
            }

            //12.קלוט שני מספרים. אם המספרים שווים הדפס " equal ,"אם המספרים שונים, הדפס את המספר הקטן יותר
            //מבניהם.
            System.out.println("Please enter number");
            int num1 = s.nextInt();
            System.out.println("Please enter number");
            int num2 = s.nextInt();

            if (num1 == num2) {
                System.out.println("equal");
            } else if (num1 < num2) {
                System.out.println(num1);
            } else
                System.out.println(num2);
        }

        // Question number 13 from the targil

        System.out.println("Please enter 3 numbers:");
        int E = s.nextInt();
        int F = s.nextInt();
        int G = s.nextInt();

        if ((E > F && E < G) || (E > G) && (E < G)) {
            System.out.println("x is the middle");
        } else if ((F > E && F < G) || (F > G && F < E)) {
            System.out.println("y is the middle");
        } else {
            System.out.println("z is the middle");
        }

        //14.קלוט שני מספרים והדפס אותם לפי הסדר )קודם הקטן, ואחר כך הגדול(. השתמש ב-format.string .
        System.out.println("Please enter number:");
        int c = s.nextInt();
        System.out.println("Please enter number:");
        int h = s.nextInt();

        //15.כתוב לולאה שמדפיסה את כל המספרים מ-0 עד 10.
        System.out.println();
        for (int index = 0; index <= 10; index++) {
            System.out.println(index);
        }

        //16.כתוב לולאה שמדפיסה את כל המספרים הלא-זוגיים מ-1 עד 50
        System.out.println();
        for (int index = 1; index <= 50; index = index + 2) {
            System.out.println(index);
        }
        //17. כתוב לולאת while do שבכל פעם מגרילה מספר באמצעות random( מ-10 עד 30 )ומדפיסה אותו, עד אשר
        //מוגרל המספר 15 - ואז הלולאה תסתיים.

        Random r = new Random();
        int hagrala;
        do {
            hagrala = r.nextInt(20) + 10;
            System.out.print(hagrala + " ");
        } while (hagrala != 15);


        //targil 18

        switch (number) {
            case 1:
                System.out.println("one");
                break;
            case 2:
                System.out.println("two");
                break;
            case 3:
                System.out.println("three");
                break;
            default:
                System.out.println("number unknown");
        }


        //19.על מנת לממש מחשבון מיוחד הסוכם סדרת מספרים -
        //כתוב לולאת (true(while שקולטת מספרים מהמשתמש עד שהוא מכניס 0 .ברגע שהוכנס 0 ,צא מהלולאה
        //והדפס את סכום המספרים שהמשתמש הכניס.


        int sum4 = 0;
        while (true) {
            System.out.println("Please insert a number");
            int num4 = s.nextInt();
            if (num4 == 0) {
                break;
            } else {
                sum += num;
            }
        }
        System.out.println("The sum is: " + sum);

        // Targil 20

        System.out.println("please insert a 3 digit number:");
        int num3 = s.nextInt();
        System.out.println("Sifrat ha-asarot: " + num3);


        // Targil 21

        int sum1 = 0, count = 0;
        while (true) {
            System.out.println("Please enter grade");
            int grade = s.nextInt();
            if (grade != -1) {
                sum1 += grade;
                count++;
            } else {
                break;
            }
        }

    }
}

