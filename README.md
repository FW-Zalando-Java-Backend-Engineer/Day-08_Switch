# **📘 Day-08: Java Switch Statement**  
Welcome to **Day-08** of our Java learning journey! Today, we will explore the powerful **`switch` statement**, a cleaner alternative to long `if-else` chains. Mastering `switch` helps improve readability and structure when making decisions based on a single value.

---

## **📌 Lesson Structure**

### **1️⃣ Introduction to the Switch Statement**
- What is a `switch` statement?
- When to use `switch` vs. `if-else`
- Supported data types (int, char, String, enums)

### **2️⃣ Basic Syntax of a Switch**
- Structure of a `switch` block
- The role of `case`, `break`, and `default`

### **3️⃣ Switch Statement Examples**
- Simple number & grade matchers
- Character and String-based switches

### **4️⃣ Fall-Through Behavior**
- What happens without a `break`
- How to intentionally allow multiple matches

### **5️⃣ Switch with Strings (Java 7+)**
- Using strings as `case` values
- Matching user input or commands

### **6️⃣ Nested Switch (Advanced)**
- Embedding a switch inside another
- Use cases: multi-level menus, role + action logic

---

## **📜 Live Coding Examples**

### **🖥️ Basic Switch Case**

```java
public class DayOfWeek {
    public static void main(String[] args) {
        int day = 3;

        switch (day) {
            case 1:
                System.out.println("Monday");
                break;
            case 2:
                System.out.println("Tuesday");
                break;
            case 3:
                System.out.println("Wednesday");
                break;
            default:
                System.out.println("Invalid day");
        }
    }
}
```

**📝 Expected Output:**
```
Wednesday
```

---

### **🖥️ Switch with String**

```java
public class CommandHandler {
    public static void main(String[] args) {
        String command = "logout";

        switch (command.toLowerCase()) {
            case "login":
                System.out.println("Logging in...");
                break;
            case "logout":
                System.out.println("Logging out...");
                break;
            case "help":
                System.out.println("Showing help menu.");
                break;
            default:
                System.out.println("Unknown command.");
        }
    }
}
```

**📝 Expected Output:**
```
Logging out...
```

---

### **🖥️ Fall-Through Behavior**

```java
public class FallThroughExample {
    public static void main(String[] args) {
        int level = 1;

        switch (level) {
            case 1:
                System.out.println("Bronze");
            case 2:
                System.out.println("Silver");
            case 3:
                System.out.println("Gold");
                break;
            default:
                System.out.println("Invalid level");
        }
    }
}
```

**📝 Expected Output:**
```
Bronze
Silver
Gold
```

---

### **🖥️ Nested Switch Example**

```java
public class NestedSwitch {
    public static void main(String[] args) {
        String role = "admin";
        int action = 2;

        switch (role) {
            case "admin":
                switch (action) {
                    case 1: System.out.println("Manage users"); break;
                    case 2: System.out.println("View reports"); break;
                    default: System.out.println("Unknown action");
                }
                break;
            case "user":
                System.out.println("User dashboard");
                break;
            default:
                System.out.println("Unauthorized role");
        }
    }
}
```

**📝 Expected Output:**
```
View reports
```

---

## **🎯 Hands-on Exercises**

✅ Create a program that matches a number to a **month name** using `switch`.  
✅ Build a **simple command-line calculator** using `switch` on the operator (`+`, `-`, `*`, `/`).  
✅ Create a **menu system** using nested `switch`: select category, then action.  
✅ Write a program that uses a **`switch` with a `String`** to simulate a basic chatbot.

---

## **🧑‍🏫 GitHub Classroom Exercises**
✅ [🏛️ Smart City Utility Portal](https://github.com/FW-Zalando-Java-Backend-Engineer/Smart-City-Utility-Portal)
✅ [🚘 Smart Toll Management System](https://github.com/FW-Zalando-Java-Backend-Engineer/Smart-Toll-Management-System)
✅ [🏛️ Smart City Utility Portal Solution - code ](https://github.com/FW-Zalando-Java-Backend-Engineer/Smart-City-Utility-Portal/tree/solution)
✅[🏛️ Smart City Utility Portal Solution - Live recording](https://us06web.zoom.us/rec/share/A-SoJdODwwzqxazDnqT6daxVLI7wsIJP4uCqbktyrXax9hlrNtlLxpCurh9g1KY.p0amjoud3cvvA-2m)

---

## **📚 Additional Resources**

- [Baeldung: Java Switch Statement](https://www.baeldung.com/java-switch)
- [freeCodeCamp: Java Switch Case Tutorial](https://www.freecodecamp.org/news/java-switch-statement-how-to-use-a-switch-case-in-java/)
- [Builtin.com: Java Switch Explained](https://builtin.com/articles/java-switch-case)
- [Codementor: Switch vs. Switch Expressions](https://www.codementor.io/@noelkamphoa/switch-statements-and-switch-expressions-in-java-the-differences-2etcvbxfaa)
- [The Knowledge Academy: Java Switch Guide](https://www.theknowledgeacademy.com/blog/switch-case-java/)
- [Jenkov Switch Tutorial](https://jenkov.com/tutorials/java/switch.html)
- [Video Lesson Recording](https://us06web.zoom.us/rec/share/A-SoJdODwwzqxazDnqT6daxVLI7wsIJP4uCqbktyrXax9hlrNtlLxpCurh9g1KY.p0amjoud3cvvA-2m)

---

🚀 **Great job! Now you're equipped to make smart decisions (in Java, at least 😉).** Get ready for even more dynamic logic tomorrow! 🎉

