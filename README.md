# Unit-of-Measurement-Converter-Project
Unit of Measurement Converter Project made in python

convert_from = input("Enter Starting Unit of Measurement(inches, feet, yards): ")

convert_to = input("Enter Starting Unit to Convert(inches, feet, yards): ")

if convert_from.lower() in ["inches","in","inch"]:
    number_of_inches = int(input("Enter Starting Measurement in Inches: "))
    if convert_to.lower() in ["feet","foot","ft"]:
        print("Result: " + str(number_of_inches) + " Inches = " + str(round(number_of_inches/ 12)) + " Feet")
    elif convert_to.lower() in ["yards", "yard","yds","yd"]:
        print("Result: " + str(number_of_inches) + " Inches = " + str(round(number_of_inches / 36)) + " Yards")
    else:
        print("Please, Enter either Inches, Feet, or Yards.")
elif convert_from.lower() in ["feet","foot","ft"]:
    number_of_feet = int(input("Enter Starting Measurement in feet: "))
    if convert_to.lower() in ["inches","in","inch"]:
        print("Result: " + str(number_of_feet) + " Feet = " + str(round(number_of_feet * 12)) + " Inches")
    elif convert_to.lower() in ["yards", "yard","yds","yd"]:
        print("Result: " + str(number_of_feet) + " Feet = " + str(round(number_of_feet / 3)) + " Yards")
    else:
        print("Please, Enter either Inches, Feet, or Yards.")
elif convert_from.lower() in ["yards", "yard","yds","yd"]:
    number_of_yards = int(input("Enter Starting Measurement in yards: "))
    if convert_to.lower() in ["inches","in","inch"]:
        print("Result: " + str(number_of_yards) + " Yards = " + str(round(number_of_yards * 36)) + " Inches")
    elif convert_to.lower() in ["feet","foot","ft"]:
        print("Result: " + str(number_of_yards) + " Yards = " + str(round(number_of_yards * 3)) + " Feet")
    else:
        print("Please, Enter either Inches, Feet, or Yards.")
else:
    print("Please, Enter either Inches, Feet, or Yards.")  
