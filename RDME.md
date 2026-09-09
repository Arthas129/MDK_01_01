#include <iostream>

int main() {
    std::cout << "C++ is a general-purpose programming language with a bias towards systems programming that\n"
        << "  - is a better C\n"
        << "  - supports data abstraction\n"
        << "  - supports object-oriented programming\n"
        << "  - supports generic programming.\n";

    // Второе задание на нахождение сумммы
    long long a, b;
    std::cin >> a >> b;
    std::cout << a + b << std::endl;

    double cm;
    std::cin >> cm;

    // Тррретье задание на дюмы
    double inches = cm / 2.54;

    std::cout << inches << std::endl;

    // Четвертое задаание на прогресию
    long long n;
    std::cin >> n;

    std::cout << n * (n + 1) / 2 << "\n";

    // Пятое задание
    int x1, y1, x2, y2;
    std::cin >> x1 >> y1 >> x2 >> y2;

    int dx = x1 - x2;
    int dy = y1 - y2;

    
    if (x1 == x2 || y1 == y2 || dx == dy || dx == -dy) {
        std::cout << "YES\n";
    }
    else {
        std::cout << "NO\n";
    }


    //6 задание
    long long side1, side2, side3;
    std::cin >> side1 >> side2 >> side3;

    if (side1 + side2 <= side3 || side1 + side3 <= side2 || side2 + side3 <= side1) {
        std::cout << "UNDEFINED\n";
    }
    else if (side1 * side1 + side2 * side2 == side3 * side3 ||
        side1 * side1 + side3 * side3 == side2 * side2 ||
        side2 * side2 + side3 * side3 == side1 * side1) {
        std::cout << "YES\n";
    }
    else {
        std::cout << "NO\n";
    }

    //7 задание
    int year;
    std::cin >> year;

    if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0)) {
        std::cout << "YES\n";
    }
    else {
        std::cout << "NO\n";
    }

    //eight задание
    int month, yeaar;
    std::cin >> month >> yeaar;

    if (month == 2) {
        
        if ((yeaar % 4 == 0 && yeaar % 100 != 0) || (yeaar % 400 == 0)) {
            std::cout << 29 << std::endl;
        }
        else {
            std::cout << 28 << std::endl;
        }
    }
    
    else if (month == 4 || month == 6 || month == 9 || month == 11) {
        std::cout << 30 << std::endl;
    }
    
    else {
        std::cout << 31 << std::endl;
    }

    // 999 задание
    long long m;
    std::cin >> m;

    long long sum = 0;

    
    while (m > 0) {
        sum += m % 10;
        m /= 10;       
    }

    std::cout << sum << std::endl;

    return 0;
}
