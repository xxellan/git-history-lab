#include <iostream>
#include <vector>
#include <limits>

using namespace std;

double findMax(const vector<double>& numbers) {
    if (numbers.empty()) {
        return numeric_limits<double>::lowest();
    }
    
    double maxValue = numbers[0];
    for (double num : numbers) {
        if (num > maxValue) {
            maxValue = num;
        }
    }
    
    return maxValue;
}