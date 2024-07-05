def celsius_to_fahrenheit(celsius):
    return (celsius * 9/5) + 32
def celsius_to_kelvin(celsius):
    return celsius + 273.15
def fahrenheit_to_celsius(fahrenheit):
    return (fahrenheit - 32) * 5/9
def fahrenheit_to_kelvin(fahrenheit):
    return (fahrenheit - 32) * 5/9 + 273.15
def kelvin_to_celsius(kelvin):
    return kelvin - 273.15
def kelvin_to_fahrenheit(kelvin):
    return (kelvin - 273.15) * 9/5 + 32
def convert_temperature():
    print("Temperature Converter")
    temp = float(input("Enter the temperature value: "))
    unit = input("Enter the unit of the temperature (C for Celsius, F for Fahrenheit, K for Kelvin): ").upper()
    if unit == 'C':
        print(f"{temp}°C is equal to {celsius_to_fahrenheit(temp):.2f}°F")
        print(f"{temp}°C is equal to {celsius_to_kelvin(temp):.2f}K")
    elif unit == 'F':
        print(f"{temp}°F is equal to {fahrenheit_to_celsius(temp):.2f}°C")
        print(f"{temp}°F is equal to {fahrenheit_to_kelvin(temp):.2f}K")
    elif unit == 'K':
        print(f"{temp}K is equal to {kelvin_to_celsius(temp):.2f}°C")
        print(f"{temp}K is equal to {kelvin_to_fahrenheit(temp):.2f}°F")
    else:
        print("Invalid unit. Please enter C for Celsius, F for Fahrenheit, or K for Kelvin.")

if __name__ == "__main__":
    convert_temperature()
