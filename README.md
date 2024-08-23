# Домашнее задание к занятию "Testability, авто-тесты, введение в ООП: объекты и методы"

## Case2
**BmiService.java**
```java
package Case2;

public class BmiService {
    public int calculate(double heightInMeters, double weightInKilograms) {
        double bmi = weightInKilograms / (heightInMeters * heightInMeters);
        return (int) bmi;
    }
}
```
**Main2.java**
```java
package Case2;

public class Main2 {
    public static void main(String[] args) {
        BmiService service = new BmiService();
        double heightInMeters = 1.87;
        double weightInKilograms = 98;
        int bmi = service.calculate(heightInMeters, weightInKilograms); // должно получиться 28
        System.out.println("bmi-индекс: " + bmi);
    }
}
```
**Результат**
```
bmi-индекс: 28
```

### Файлы с кодом можно посмотреть в [папке](https://github.com/AngryCFO/Testability/tree/main/src)

