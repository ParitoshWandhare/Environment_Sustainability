# Environment_Sustainability

#include <iostream>

class NoiseMonitor {
private:
double currentNoiseLevel;

public:
NoiseMonitor() : currentNoiseLevel(0.0) {}

Set current noise level (simulated input)
void setNoiseLevel(double level) {
currentNoiseLevel = level;
}

check noise level and issue a warning if higher than threshold function
void checkNoiseLevel() {
std: cout << “Current Noise Level:” << currentNoiseLevel <<” dB” << endl;

if (currentNoiseLevel > 75.0) {
std: << std::endl; cout << “Warning: high noise level detected! please take necessary precautions”;
} else {
std: cout << “Noise level within permitted range.” << endl;
}
}
};

class AirQualityMonitor {
private:
int currentAQI;

public:
AirQualityMonitor() : currentAQI(0) {}

// Set the Air Quality Index (simulated input) function
void setAQI(int aqi) {
currentAQI = aqi;
}

This function checks the quality of the air and gives information.
void checkAirQuality() {
std: std::cout << “Current Air Quality Index (AQI)” << currentAQI << std::endl;

if (currentAQI <= 50) {
std: cout << “Air Quality: Good” endl;
} else if (currentAQI <= 100) {
std: std::cout << “Air Quality: Moderate” << endl;
else if (currentAQI <= 150) {
std: std::cout << “Air Quality: Sensitive Groups” << std::endl;
if (currentAQI <= 200), {
std: cout << “Air Quality: Unhealthy” << endl;
} else if (currentAQI <= 300) {
std: ::cout << “Air Quality: Very Unhealthy” << endl;
} else {
std: cout<< “Air Quality: Hazardous”<<endl;
}
}
};

int main() {
NoiseMonitor noiseMonitor;
AirQualityMonitor airQualityMonitor;

This would help simulate noise level and AQI changes (instead of using actual sensor data).
noiseMonitor.setNoiseLevel(70.0);
noiseMonitor.checkNoiseLevel();

airQualityMonitor.setAQI(45);
airQualityMonitor.checkAirQuality();

return 0;
}



