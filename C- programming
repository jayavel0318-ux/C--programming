#include <stdio.h>

/* 1. Cab Fare Calculation */
void q1() {
    int distance, member;
    float fare = 100;
    printf("Distance: ");
    scanf("%d", &distance);
    printf("Member (1 = true, 0 = false): ");
    scanf("%d", &member);
    if (distance > 10)
        fare += 20 * (distance - 10);
    if (member)
        fare *= 0.9;
    printf("Final Fare: Rs.%g\n", fare);
}

/* 2. Online Examination System */
void q2() {
    int answered, remaining, submitted;
    printf("Questions Answered, Remaining Time, Already Submitted: ");
    scanf("%d %d %d", &answered, &remaining, &submitted);
    if (answered >= 1 && remaining > 0 && submitted == 0)
        printf("Submission Allowed\n");
    else
        printf("Submission Not Allowed\n");
}

/* 3. Treasure Hunt */
void q3() {
    int total, x, y;
    printf("Total coins, x%%, y%%: ");
    scanf("%d %d %d", &total, &x, &y);
    int ben = total * x / 100;
    int remaining = total - ben;
    int blackbeard = remaining * y / 100;
    remaining -= blackbeard;
    int each = remaining / 3; /* leftover coins thrown into the sea */
    printf("%d\n%d\n%d\n", ben, blackbeard, each);
}

/* 4. Dollars & Cents */
void q4() {
    int d1, c1, d2, c2;
    printf("Dollar1 Cent1 Dollar2 Cent2: ");
    scanf("%d %d %d %d", &d1, &c1, &d2, &c2);
    int cents = c1 + c2;
    int dollars = d1 + d2 + cents / 100;
    cents = cents % 100;
    printf("%d\n%d\n", dollars, cents);
}

/* 5. Car Mileage */
void q5() {
    float mileage;
    int petrol, distance;
    printf("Mileage, Petrol (litres), Distance: ");
    scanf("%f %d %d", &mileage, &petrol, &distance);
    if (mileage * petrol >= distance)
        printf("Can reach\n");
    else
        printf("Cannot reach\n");
}

/* 6. Car Race */
void q6() {
    int a, b, c, car;
    printf("Road A, Road B, Road C, Car number: ");
    scanf("%d %d %d %d", &a, &b, &c, &car);
    if (a % car == 0)
        printf("Car 1 goes into road A\n");
    else if (b % car == 0)
        printf("Car 1 goes into road B\n");
    else if (c % car == 0)
        printf("Car 1 goes into road C\n");
    else
        printf("No path exists\n");
}

/* 7. Debt Repay */
void q7() {
    int p, r, n;
    printf("Principal, Rate, Years: ");
    scanf("%d %d %d", &p, &r, &n);
    float interest = (float)p * r * n / 100;
    float amount = p + interest;
    float discount = interest * 0.02;
    float settlement = amount - discount;
    printf("%.2f\n%.2f\n%.2f\n%.2f\n", interest, amount, discount, settlement);
}

/* 8. Employee Job Level */
void q8() {
    int exp, perf;
    printf("Experience: ");
    scanf("%d", &exp);
    printf("Performance: ");
    scanf("%d", &perf);
    if (exp < 3)
        printf("Level: Junior\n");
    else if (exp <= 7) {
        if (perf >= 80)
            printf("Level: Mid-Level\n");
        else
            printf("Level: Junior\n");
    } else {
        if (perf >= 85)
            printf("Level: Senior\n");
        else if (perf >= 80)
            printf("Level: Mid-Level\n");
        else
            printf("Level: Junior\n");
    }
}

/* 9. Number of Days */
void q9() {
    int year, month, days;
    printf("Year Month: ");
    scanf("%d %d", &year, &month);
    if (year < 1900 || year > 9999) {
        printf("0\n");
        return;
    }
    switch (month) {
        case 1: case 3: case 5: case 7: case 8: case 10: case 12:
            days = 31; break;
        case 4: case 6: case 9: case 11:
            days = 30; break;
        case 2:
            if ((year % 4 == 0 && year % 100 != 0) || year % 400 == 0)
                days = 29;
            else
                days = 28;
            break;
        default:
            printf("0\n");
            return;
    }
    printf("%d Days\n", days);
}

/* 10. Electricity Bill */
void q10() {
    int units;
    float bill;
    printf("Units: ");
    scanf("%d", &units);
    if (units <= 200)
        bill = units * 0.5;
    else if (units <= 400)
        bill = units * 0.65 + 100;
    else if (units <= 600)
        bill = units * 0.80 + 200;
    else
        bill = units * 1.25 + 425;
    printf("Rs.%g\n", bill);
}

int main() {
    int choice;
    printf("Enter question number (1-10): ");
    scanf("%d", &choice);
    switch (choice) {
        case 1: q1(); break;
        case 2: q2(); break;
        case 3: q3(); break;
        case 4: q4(); break;
        case 5: q5(); break;
        case 6: q6(); break;
        case 7: q7(); break;
        case 8: q8(); break;
        case 9: q9(); break;
        case 10: q10(); break;
        default: printf("Invalid question number\n");
    }
    return 0;
}
