# Reverse Me

![Untitled](Reverse%20Me%20df87340b3d184d32a70d9fc7fe50fec7/Untitled.png)

```powershell
import java.util.*;

public class JavaRev {
    public static void main(String args[]) {
        JavaRev vaultDoor = new JavaRev();
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter vault password: ");
        String userInput = scanner.next();
        String input = userInput.substring("CTF{".length(), userInput.length() - 1);
        if (vaultDoor.checkPassword(input)) {
            System.out.println("Access granted.");
        } else {
            System.out.println("Access denied!");
        }
        scanner.close();
    }

    public boolean checkPassword(String password) {
        return password.length() == 25 &&
                password.charAt(0) == 'u' &&
                password.charAt(4) == 'r' &&
                password.charAt(2) == '5' &&
                password.charAt(23) == 'r' &&
                password.charAt(3) == 'c' &&
                password.charAt(17) == '@' &&
                password.charAt(1) == 'n' &&
                password.charAt(7) == 'b' &&
                password.charAt(10) == '_' &&
                password.charAt(5) == '@' &&
                password.charAt(9) == '3' &&
                password.charAt(11) == 't' &&
                password.charAt(15) == 'c' &&
                password.charAt(8) == 'l' &&
                password.charAt(12) == 'h' &&
                password.charAt(20) == 'c' &&
                password.charAt(14) == '_' &&
                password.charAt(6) == 'm' &&
                password.charAt(24) == '5' &&
                password.charAt(18) == 'r' &&
                password.charAt(13) == '3' &&
                password.charAt(19) == '@' &&
                password.charAt(21) == 't' &&
                password.charAt(16) == 'h' &&
                password.charAt(22) == '3';
    }
}
```

This was an easy challenge It checks for a password and if the password is right or is flag it says "Access granted." else give "Access denied!”.

Looking at the code we know that it has a password of 25 characters and the it starts with CTF{.

After that, by looking at the value at charAt(x) we can rewrite the flag.

After analysing the indexing of the variable in a format [i.e.  charAt(x)].

```powershell
CTF{un5cr@mbl3_th3_ch@r@ct3r5}
```

![Untitled](Reverse%20Me%20df87340b3d184d32a70d9fc7fe50fec7/Untitled%201.png)