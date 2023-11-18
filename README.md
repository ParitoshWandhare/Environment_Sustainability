# Environment_Sustainability
#include <iostream>

class NoiseMonitor {
private:
    double currentNoiseLevel;

public:
    NoiseMonitor() : currentNoiseLevel(0.0) {}

    // Function to set the current noise level (simulated input)
    void setNoiseLevel(double level) {
        currentNoiseLevel = level;
    }

    // Function to check the noise level and give a warning if it's above the threshold
    void checkNoiseLevel() {
        std::cout << "Current Noise Level: " << currentNoiseLevel << " dB" << std::endl;

        if (currentNoiseLevel > 75.0) {
            std::cout << "Warning: High Noise Level Detected! Please take necessary precautions." << std::endl;
        } else {
            std::cout << "Noise level within acceptable range." << std::endl;
        }
    }
};

class AirQualityMonitor {
private:
    int currentAQI;

public:
    AirQualityMonitor() : currentAQI(0) {}

    // Function to set the current Air Quality Index (simulated input)
    void setAQI(int aqi) {
        currentAQI = aqi;
    }

    // Function to check the air quality and provide corresponding information
    void checkAirQuality() {
        std::cout << "Current Air Quality Index (AQI): " << currentAQI << std::endl;

        if (currentAQI <= 50) {
            std::cout << "Air Quality: Good" << std::endl;
        } else if (currentAQI <= 100) {
            std::cout << "Air Quality: Moderate" << std::endl;
        } else if (currentAQI <= 150) {
            std::cout << "Air Quality: Unhealthy for Sensitive Groups" << std::endl;
        } else if (currentAQI <= 200) {
            std::cout << "Air Quality: Unhealthy" << std::endl;
        } else if (currentAQI <= 300) {
            std::cout << "Air Quality: Very Unhealthy" << std::endl;
        } else {
            std::cout << "Air Quality: Hazardous" << std::endl;
        }
    }
};

int main() {
    NoiseMonitor noiseMonitor;
    AirQualityMonitor airQualityMonitor;

    // Simulate noise level and AQI changes (replace this with actual sensor data)
    noiseMonitor.setNoiseLevel(70.0);
    noiseMonitor.checkNoiseLevel();

    airQualityMonitor.setAQI(275);
    airQualityMonitor.checkAirQuality();

    return 0;
}


