# Taking-Inputs
I totally get what you're saying! Taking input in different formats can be confusing at times, especially when coding under pressure in contests or interviews. Let me break it down in **the easiest and most structured way** so that you can always know what to do.  

---

## **🚀 Simple Guide for Taking Input in Java**
### **Case 1️⃣: Single Integer Input**
✅ **Example:**  
Input:  
```
5
```
Code:
```java
Scanner sc = new Scanner(System.in);
int n = sc.nextInt();
System.out.println(n);
```
---

### **Case 2️⃣: Two Integer Inputs (A, B)**
✅ **Example:**  
Input:  
```
10 20
```
Code:
```java
int a = sc.nextInt();
int b = sc.nextInt();
System.out.println(a + " " + b);
```
---

### **Case 3️⃣: Multiple Space-Separated Integers (Array Input)**
✅ **Example:**  
Input:  
```
1 2 3 4 5
```
Code:
```java
int n = sc.nextInt(); // First take the size
int[] arr = new int[n];

for (int i = 0; i < n; i++) {
    arr[i] = sc.nextInt();
}
```
---

### **Case 4️⃣: Multiple Lines (Each Line has One Integer)**
✅ **Example:**  
Input:  
```
10
20
30
40
```
Code:
```java
while (sc.hasNextInt()) {
    int num = sc.nextInt();
    System.out.println(num);
}
```
---

### **Case 5️⃣: Taking a Full Line as a String**
✅ **Example:**  
Input:  
```
Hello, I am learning Java!
```
Code:
```java
String str = sc.nextLine();
System.out.println(str);
```
---

### **Case 6️⃣: Taking Space-Separated Integers in a Single Line (Using `split()`)**
✅ **Example:**  
Input:  
```
5 10 15 20 25
```
Code:
```java
String[] input = sc.nextLine().split(" "); // Splitting based on space
int[] arr = new int[input.length];

for (int i = 0; i < input.length; i++) {
    arr[i] = Integer.parseInt(input[i]);
}
```
---

### **💡 Summary**
| Input Type                | Code |
|---------------------------|------|
| Single Integer            | `int n = sc.nextInt();` |
| Two Integers (A, B)       | `int a = sc.nextInt(); int b = sc.nextInt();` |
| Array Input (Space-Separated) | `for (int i = 0; i < n; i++) { arr[i] = sc.nextInt(); }` |
| Multi-Line Input          | `while (sc.hasNextInt()) { int num = sc.nextInt(); }` |
| Full Line as String       | `String str = sc.nextLine();` |
| Space-Separated Integers (Using Split) | `String[] input = sc.nextLine().split(" ");` |

---

## **🔑 Trick to Never Get Confused**
1️⃣ **First check if input is space-separated or line-separated.**  
2️⃣ **If it's a number first, treat it as `n` and then read `n` elements.**  
3️⃣ **If it's a full sentence, use `sc.nextLine()`.**  
4️⃣ **If stuck, print intermediate results (`System.out.println()`) to debug.**  

---

Now you **never** have to worry about input formats again! 🚀 Keep practicing, and it'll become second nature. 😊
