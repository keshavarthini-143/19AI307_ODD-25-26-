# Ex.No:4(B)  IMPLEMENT SOLID PRINCIPLES IN JAVA PROGRAM 

## QUESTION:
In a gaming lounge, there is only one master console power switch that controls all gaming consoles. Whenever a player turns on any console, it internally triggers the master power. The master switch must ensure only one instance is ever created, regardless of how many times it's accessed, to prevent power fluctuations.
Every time a player accesses the master switch, it logs an access count. Since the switch is Singleton, the count should increment globally and reflect shared state.

## AIM:
To develop a Java program that manages a master console power switch shared by all gaming consoles and maintains a common access count whenever a player accesses it.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a class to manage the Master Power Switch.
4. Ensure that the same Master Power Switch is shared whenever it is accessed.
5. Initialize the access count to zero.
6. Read the number of players.
7. For each player, read the player's name.
8. Access the Master Power Switch.
9. Increment the common access count.
10. Display the player's name and the total number of accesses so far.
11. Repeat the process for all players.
12. Stop the program.


## PROGRAM:
 ```
/*
Program to implement a SOLID Principles in Java Program
Developed by: KESHAVARTHINI B
RegisterNumber: 212224040158
*/
```

## SOURCE CODE:
```
import java.util.*;

class MasterPowerSwitch {
    private static MasterPowerSwitch instance;
    private int count;
    private MasterPowerSwitch(){
        this.count=0;
    }
    public static MasterPowerSwitch getInstance(){
        if(instance==null){
            instance=new MasterPowerSwitch();
        }
        return instance;
    }
    public int logAccess(){
        this.count++;
        return this.count;
    }
}

public class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < n; i++) {
            String player = sc.nextLine();
            MasterPowerSwitch power = MasterPowerSwitch.getInstance();
            int count = power.logAccess();
            System.out.println(player + " accessed Master Power Switch. Total accesses so far: " + count);
        }
    }
}

```


## OUTPUT:

<img width="1246" height="255" alt="image" src="https://github.com/user-attachments/assets/f762f799-860e-46ab-999e-46b5c390160d" />


## RESULT:
The program was executed successfully. The Master Power Switch was shared among all players, and the access count was updated globally for each access.
