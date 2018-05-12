```
$ echo "public class Main {public static void main(String[] args) {System.out.println("Hello World!");}}" >> Main.java
$ coala --files Main.java --bears=LineCountBear,SpaceConsistencyBear --save
Please enter a value for the setting "max_lines_per_file" (Number of lines allow            ed per file.) needed by LineCountBear for section "cli":
5
Please enter a value for the setting "use_spaces" (True if spaces are to be used             instead of tabs.) needed by SpaceConsistencyBear for section "cli":
True
Executing section cli...

main.java
|   2| »   public·static·void·main(String[]·args)·{
|    | [NORMAL] SpaceConsistencyBear:
|    | Line contains following spacing inconsistencies:
|    | - Tabs used instead of spaces.
|----|    | e:\personal projects\open source\coala_java_example\main.java
|    |++++| e:\personal projects\open source\coala_java_example\main.java
|   1|   1| public class Main {
|   2|    |-    public static void main(String[] args) {
|    |   2|+    public static void main(String[] args) {
|   3|   3|             System.out.println(Hello World >> main.java);
|   4|   4|             }
|   5|   5|             }
|    | *0: Do nothing
|    |  1: Open file(s)
|    |  2: Apply patch
|    |  3: Add ignore comment
|    | Enter number (Ctrl-Z to exit): 2
|    | Patch applied successfully.
```
