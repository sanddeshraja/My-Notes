In CMD : set path =c:\pgm files\java\jdk-14.0.1\bin;%path%;

Scanner obj = new Scanner(System.in);
int a;
a=obj.nextInt();
ASCII - American Standard code of Information Interchange

Variables rules

case sensitive
has alpha,num, _ ,$
my start with _ $
no keywords

| Interpreter                                   | Compiler                      |
| --------------------------------------------- | ----------------------------- |
| Doesnot create a new file                     | Creates a new File            |
| line by line                                  | All at once                   |
| After translate need everytime u run the cose | no need compiler all the time |


JAVA IS PLATFORM INDEPENDENT

![[JAVA 2022-11-02 15.12.51.excalidraw]]


Coercion internal convertion of data from one type to other

byte+short =int
short +int=int
int +float=float
long+float=float
char+short=int
char+int=int
float+double=double

## bit wise operation

and &
1 & 1 = 1
1 & 0 =0
0 & 1 =0
0 & 0 = 0

or |
1 | 1 =1
1 | 0 =1
0 | 1 =1
0 | 0 =0

xor ^

1^0=1
0^1=1
0^0=0
1^1=0

left shift (x<<1) will give 2x for 1
right shift (x>>1) will give x/2 for 1
for signed right shift firast convert the number to 2s complement(+ve to 2s comlement) and perform right shift
prefferd to watch video


## VARIABLE LENGTH ARGUMENTS

static void fun(int ...v){
System.out.println(Arrays.toString(v));
}

## 2D Array
<code>
int[ ][ ] arr = new int[3][3];
</code>

<code>int[][] arr={
{1,2,3},
{4,5,6},
{7,8,9}
};
</code>

Row must be mentioned Column is optional

No call by reference in Java


## ArrayList(Collection Framework)

when you don't know the size
<code>
ArrayList &lt;Integer&gt;  list = new ArrayList &lt;&gt;(10);
</code>
list.add(67);
System.out.println(list);
list.contains(654); //False
list.set(0,68);
list.remove(0);
list.get(0);


to use for each you need a collection

(int)(Math.log10(num))+1 gives total digits in a given num

