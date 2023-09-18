#CS4141 
Reccommended IDE: BlueJ

---
## java.lang
basic tools (Math, String, System)
```java
import java.lang.System; //Specific
import java.lang.Math; //Specific
//OR
import java.lang.*; //ALL
```

---
## System.out
- `System.out.print(...); //Prints to output`
- `System.out.println(...); //Prints to output then moves to next line`
- `System.out.println("5 times 9 is " + 5*9)`
	```java
	System.out.print("7 + 12 is " + 7 + 12); 
	//Output
	//7 + 12 is 712
	System.out.print("7 + 12 is " + (7 + 12));
	//Output
	//7 + 12 is 19
```

---
## System.currentTimeMillis()
Returns number of milliseconds since January 1st 1970.
- Number of milliseconds in a day:
	`24*60*60*1000`
- Number of days since 1 Jan 1970:
	`System.currentTimeMillis() / (24*60*60*1000)`
- Number of milliseconds since midnight last night: 
	`System.currentTimeMillis() % (24*60*60*1000)`

---
## System.getProperty(key)

Common keys:
- `java.version`
- `java.home`
- `os.name`
- `os.version`
- `user.name`
- `user.home`
- `user.dir`

