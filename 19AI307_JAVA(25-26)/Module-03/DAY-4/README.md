# Ex.No:3(D)    INTERFACE 

## QUESTION:
You are programming bots that analyze weather data. Each bot must implement a common interface and give a prediction.

 Bot Types:

SunBot: Predicts "HOT" if temperature > 30, else "MODERATE".

RainBot: Predicts "COLD" if temperature < 20, else "WARM".

## AIM:
To demonstrate interface-based polymorphism by creating a common WeatherBot interface and implementing it using SunBot and RainBot.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a WeatherBot interface with the predict() method and implement it in SunBot and RainBot.
4. Read the temperature and bot type from the user.
5. Create the appropriate bot object based on the bot type.
6. Call predict() and display the weather prediction.

## PROGRAM:
 ```
/*
Program to implement a Interface using Java
Developed by: KESHAVARTHINI B
RegisterNumber:  212224040158
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

interface WeatherBot {
    String predict(int temperature);
}

class SunBot implements WeatherBot {

    public String predict(int temperature) {

        if (temperature > 30) {
            return "HOT";
        } else {
            return "MODERATE";
        }
    }
}

class RainBot implements WeatherBot {

    public String predict(int temperature) {

        if (temperature < 20) {
            return "COLD";
        } else {
            return "WARM";
        }
    }
}

public class Main {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int temperature = sc.nextInt();
        int botType = sc.nextInt();

        WeatherBot bot;

        if (botType == 1) {
            bot = new SunBot();
        } else {
            bot = new RainBot();
        }

        System.out.println(bot.predict(temperature));

        sc.close();
    }
}
```


## OUTPUT:

<img width="400" height="168" alt="image" src="https://github.com/user-attachments/assets/fc4c6238-5c9f-4ac7-bf0a-a0e7f60d7c2e" />


## RESULT:
Thus, the Java program successfully demonstrates interface implementation and polymorphism to generate weather predictions.
