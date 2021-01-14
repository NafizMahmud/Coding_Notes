### Reflection:
Java reflection hoilo onno class er private method search korar system.. Interesting.. Normally ek class e onno class er object declare korleo private method acces kora jai na. Tai reflection use kora hoi. System hoilo oi class er object declare kore then Method name class er obj k oi class er method er description assign kora.. Taile oi Method Class er obj oi private method khuje ber kore tar reflection nijer moddhe niye bose ase.. Then oi Method class er obj named method k invoke korelei access but aita real oi private function na.. Just oi function er ekta reflection niya asche.
```java
A a = new A();
Method m = A.class.getDeclaredMethod("get", new Class[] { String.class, Date.class });
m.setAccessible(true);
```

### Throw,Throws: 
Throws hoilo akta code block exception throw korte paare sei declaration. 

***Oi block er code or method jodi keu onno jaiga theke call kore thake setake obossoi exception handle korte hobe.
  ```java
  void m()throws IOException{  
throw new IOException("device error");//checked exception  }  
  void p(){ try{ m(); }
catch(Exception e){System.out.println("exception handled");}   }
p(); // er moddhe try catch khela laagbei.
```
VVI:
jodi eclipse er moddhe kkhno debug clear na hoi f5 try kore dekha jete paare..f5 hoilo exactly koi koi gese sob ghurbe… f6 joto method e call hok na just porer line e jabe...   

### Review Exception --
1.Checked Exception holo easiest. Code lekhar somoi eclipse bolbe aita dame...try catch na kore compile e hobe na. FileNotFoundException - oi File k access koro declare korle sathe sathe file check kore jodi na pai error dkhabe. Parse Exception same. Jekhane parse laagbe agei bole dibe Eclipse. 

2.Unchecked Exception hoilo RuntimeException. Pera bshi.  Code lekhar somoi bolbe na.. Bhalo kore chinta kore code lekha laagbe je ai block e exception hoite pare naki. Naile program kore bose thakbe.bapok pera hoilo NullPointerException or an IllegalArgumentException or ArrayIndexOutOfBoundsException.try catch or Throws use kora lagbee.

Error - Something severe enough has gone wrong the most applications should crash rather than try to handle the problem

