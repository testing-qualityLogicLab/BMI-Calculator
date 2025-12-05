# 🧮 BMI Calculator (Java)

This is a simple **console-based BMI (Body Mass Index) Calculator** written in Java.
It allows the user to enter their **weight in pounds** and **height in meters**, converts the weight to kilograms, calculates BMI, and displays their weight category.

---

## 📌 Features

* Input weight in **pounds**

* Automatic conversion from **pounds to kilograms**

* Calculates BMI using the formula:

  ```
  BMI = weight (kg) / height (m)^2
  ```

* Determines BMI category:

  * Underweight
  * Healthy weight
  * Overweight
  * Ob obese

* User-friendly console prompts

---

## 🛠️ Technologies Used

* **Java**
* **Scanner** class for reading user input

---

## 🚀 How to Run the Program

1. Make sure Java JDK (8 or above) is installed.

2. Save the file as `BMICalculator.java` inside the `day3` package folder.

3. Open a terminal and navigate to your project directory.

4. Compile the program:

   ```bash
   javac day3/BMICalculator.java
   ```

5. Run the program:

   ```bash
   java day3.BMICalculator
   ```

---

## 📂 Program Flow

1. User enters **weight in pounds**
2. User enters **height in meters**
3. Program converts pounds → kilograms using:

   ```
   kg = pounds * 0.45359237
   ```
4. BMI is calculated:

   ```
   BMI = weight(kg) / (height * height)
   ```
5. The program prints the BMI value and the corresponding category:

   * **BMI < 18.5** → Underweight
   * **18.5–24.9** → Healthy
   * **25–29.9** → Overweight
   * **30+** → Obese

---

## 🧾 Example Output

```
Enter your weight in Pounds:
150
Enter your height in meters:
1.70
Your weight in Kgs is: 68.0388555
Your BMI is: 23.54
You are Healthy weight
```

---

## 🔧 Code Snippet

```java
double weightInKgs = weightInPounds * 0.45359237;
double bmi = weightInKgs / (height * height);

if (bmi < 18.5) {
    System.out.println("You are Underweight");
} else if (bmi >= 18.5 && bmi < 24.9) {
    System.out.println("You are Healthy weight");
} else if (bmi >= 25 && bmi < 29.9) {
    System.out.println("You are Overweight");
} else {
    System.out.println("You are Obese");
}
```

---

## 📘 Notes

* Ensure inputs are valid numeric values to avoid runtime errors.
* You can enhance the program by adding:

  * Input validation
  * Support for feet/inches
  * A loop to calculate multiple BMIs
  * Color-coded console output

---

## 📜 License

This project is intended for learning and can be used freely.

---

Just tell me!
