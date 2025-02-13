# **2025-OBJPROG-LAB009**
Week 03-04 - Conditional and Looping Statements

Laboratory # 09 - Guided Coding Exercise 3: Switch Statement

## **Instructions**

### **Step 1.1: Accept the Assignment**

   1. Click on the assignment link provided by your instructor.
   2. GitHub Classroom will create a **private repository** under your GitHub account.
   3. After the repository is created, click **"Go to Repository"** to view your assignment.

---

### **Step 1.2: Setup your Git Environment**
Only perform this if this is the first time you will setup your Git Environment

   1. Create a GitHub Account:
   ```bash
   https://github.com/signup?source=login
   ```
      
   2. Download and Install Git on your Laptop/Desktop:
   ```bash
   https://git-scm.com/downloads
   ```
   
   3. Create a Folder in your Laptop/Desktop
   4. Right-click anywhere in the created folder and select "Open Git Bash Here".
   5. In the Git Bash Terminal, set your git name, perform command:
   ```bash
   git config --global user.name "Your Name"
   ```
   
   6. In the Git Bash Terminal, set your git email, perform command:
   ```bash
   git config --global user.email "your.email@example.com"
   ```
   
   7. Create your SSH Key, just follow the instructions, no need to provide filename and passphrase. In the Git Bash Terminal, perform command:
   ```bash
   ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
   ```
   
   8. Copy your SSH Keys into clipboard. In the Git Bash Terminal, perform command:
   ```bash
   clip < ~/.ssh/id_rsa.pub
   ```
   
   9. Log in to your GitHub account.
   10. In the upper-right corner of GitHub, click your profile picture and select Settings.
   11. In the left sidebar, click on SSH and GPG keys.
   12. Click the New SSH key button.
   13. In the Title field, give the key a recognizable name (e.g., "My Windows Laptop").
   14. In the Key field, CTRL + V or paste the keys copied into your clipboard. Save the key.
   15. Go Back to terminal, use command:
   ```bash
   ssh -T git@github.com
   ```

### **Step 2: Clone the Repository to Your Local Machine**

   1. On your repository page, click the green **"Code"** button.
   2. Copy the repository URL (choose HTTPS for simplicity).
   3. Open your terminal (or Git Bash, Command Prompt, or PowerShell) and run:
   
   ```bash
   git clone <git_repo_url>
   ```
   
   4. Navigate into the cloned folder:
   
   ```bash
   cd <git_cloned_folder>
   ```

### **Step 3: Complete the Assignment**

**Laboratory # 09 - Guided Coding Exercise 3: Switch Statement**

   **Objective:**
   - Learn to implement multi-conditional selection using switch statements.
   - Compare switch-case with if-else for specific scenarios.

   **File Naming Convention:**
   - `SwitchStatementDemo.java`

   **Desired Output (with day = 4 and grade = 'B'):**
   ```txt
   Thursday: Almost there.
   Good job!
   ```

   **Notable Observations (to be discussed after completing the exercise):**
   - switch statements are efficient for checking a single variable against multiple discrete values.
   - break statements are crucial to prevent fall-through.

   **Java Programming Best Practices:**
   - Use descriptive variable names.
   - Comment your code.
   - Always include break statements (unless fall-through is intended).
   - Use a default case.
      
   **Step-by-Step Instructions:**

   1. Setup Class and Main Method
      - Create a file named `SwitchStatementDemo.java`.
      - Define the class `SwitchStatementDemo` and its `main` method.
      ```Java
      public class SwitchStatementDemo {
          public static void main(String[] args) {
      
          }
      }
      ```
            
   2. Declare Day Variable (Integer)
   - Inside the main method, declare an integer variable named dayOfWeek.
   - Initialize dayOfWeek to 4 (representing Thursday).
      ```Java
      int dayOfWeek = 4;
      ```

   3. Switch Statement for Day of the Week
      - Write a switch statement using dayOfWeek as the expression.
      - Create case labels for each day of the week (1 to 7).
      - Inside each case block, print a message related to that day.
      - Add a break statement at the end of each case block.
      - Include a default case to handle invalid day numbers.
      ```Java
      switch (dayOfWeek) {
          case 1:
              System.out.println("Monday: Start of the work week.");
              break;
          case 2:
              System.out.println("Tuesday: Keep going!");
              break;
          case 3:
              System.out.println("Wednesday: Midweek.");
              break;
          case 4:
              System.out.println("Thursday: Almost there.");
              break;
          case 5:
              System.out.println("Friday: Weekend is near.");
              break;
          case 6:
              System.out.println("Saturday: Enjoy your day off!");
              break;
          case 7:
              System.out.println("Sunday: Rest and recharge.");
              break;
          default:
              System.out.println("Invalid day.");
      }
      ```

   4. Declare Grade Variable (Character)
      - Declare a character variable named studentGrade.
      - Initialize studentGrade to 'B'.
      ```Java
      char studentGrade = 'B';
      ```

   5. Switch Statement for Grade Evaluation
      - Write a switch statement using studentGrade as the expression.
      - Create case labels for each letter grade ('A', 'B', 'C', 'D', 'F').
      - Inside each case block, print a message appropriate for that grade.
      - Include break statements in each case.
      - Add a default case for invalid grades.
      ```Java
      switch (studentGrade) {
          case 'A':
              System.out.println("Excellent!");
              break;
          case 'B':
              System.out.println("Good job!");
              break;
          case 'C':
              System.out.println("Well done!");
              break;
          case 'D':
              System.out.println("You passed.");
              break;
          case 'F':
              System.out.println("Better luck next time.");
              break;
          default:
              System.out.println("Invalid grade.");
      }
      ```

   6. Compile and Run
       - Save the file as `SwitchStatementDemo.java`.
       - Compile the code using `javac SwitchStatementDemo.java` in your terminal or command prompt.
       - Run the compiled code using `java SwitchStatementDemo`.

   **Conclusion**
   This exercise demonstrates the use of switch statements for multi-conditional selection. switch statements are a clean and efficient way to handle multiple choices based on a single value.  They are particularly useful when dealing with a fixed set of values, improving code readability and maintainability. Remember the importance of break statements and the default case for robust and predictable code.  Consider switch statements as a good alternative to long if-else chains when appropriate.

### **Step 4: Push Changes to GitHub**
Once you've completed your changes, follow these steps to upload your work to your GitHub repository.

1. Check the status of your changes:
   Open the terminal and run:
   
   ```bash
   git status
   ```
   This command shows any modified or new files.
   
2. Stage the changes:
   Add all modified files to staging:
   
   ```bash
   git add .
   ```
   
3. Commit your changes:
   Write a meaningful commit message:
   
   ```bash
   git commit -m "Submitting OBJPROG Week 04 - Session 01 - Exercise 03"
   ```
   
4. Push your changes to GitHub:
   Upload your changes to your remote repository:
   
   ```bash
   git push origin main
   ```
