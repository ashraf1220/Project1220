# Project1220
//File Name StudentList.java
import java.text.*;
import java.until.*;
public class StudentList{
public static void main(String[]args){
// check arguments
if(args[0].equals("a"){
Ststem.out.println("Loading data...");
try{
BuffeReader s = new BufferReader(
new InputStreamReader(
new FileInputStream("students.txt")));
String r = s.readLine(); String i[] = r.spilt(",");
for (String j:i){System.out.println(j);}
} catch (Exception e){}
System.out.println("Data Loaded."):
}
else if(args[0].equals("r"))
{
System.out.println("Loaded data...");
try{
BuffeReader s = new BufferReader(
new InputStreamReader(
new FileInputStream("students.txt")));
String r = s.readLine(); System.out.println(r)
String i[] = r.spilt(",");
Random x = new Random();
int y = x.next.Int();
System.out.println(i[y]);
} catch (Exception e){}
System.out.println("Data Loaded."):
}
else if(args[0].contains(+))
{
System.out.println("Loaded data...");
try{
BuuferedWriter s = new BuuferedWriter(
new FileWriter("students.txt",true));
String t = args[0].substring(1);
Data d = new Data();
String df = "dd/mm/yyyy-hh:mm:ss a";
DateFormat dateFormat = new SimpleDateForamt(df);
String fd= dateFormat.format(d);
s.write(", "+t+"\nList last updated on "+fd);
s.close();
} catch (Exception e){}
System.out.println("Data Loaded."):
}
else if(args[0].contains(?))
{
System.out.println("Loaded data...");
try{
BuffeReader s = new BufferReader(
new InputStreamReader(
new FileInputStream("students.txt")));
String r = s.readLine(); 
String i[] = r.spilt(",");
boolean done = false;
String t =args[0].substring(1);
for (int idx =0; idx<i.length && !done; idx++){
if(i[idx].equals(t)){
System.out.println("We found it!");
done = true;
}
}
} catch (Exception e){}
System.out.println("Data Loaded."):
}
else if(args[0].contains(c))
{
System.out.println("Loaded data...");
try
{
BuffeReader s = new BufferReader(
new InputStreamReader(
new FileInputStream("students.txt")));
String D = s.readLine();
char a[] = D.toCharArray();
boolean in_word = false;
int count=0;
for (char c:a) {
if (c==' ')
{
if (!in_word) { count++; in_word = true:   }
else {  in_word=false;}
}
}
System.out.println(count +"word(s) found" + a.length);
} catch (Exception e){}
System.out.println("Data Loaded."):
}
}
}
