# lab2
#This program uses functions and variables

#the main function
def main():
    print ('Welcome to the meal calculator program')
    print   #prints a blank line

    #calls fuctions
    mealPrice = input_meal()
    tip = calc_tip(mealPrice)
    tax = calc_tax(mealPrice)
    total = calc_total(mealPrice,tip,tax)
    print_info(mealPrice,tip,tax,total)

#this function will input meal price
def input_meal():
    mealPrice = input("Enter meal price:")
    mealPrice = float(mealPrice)
    return mealPrice

#this function will calculate tip at 20%
def calc_tip(mealPrice):
    tip = mealPrice * .20
    return tip

#this function will calculate tax at 6%
def calc_tax(mealPrice):
    tax = mealPrice * .06
    return tax

#this function will calculate tip, tax, and the total #cost
def calc_total(mealPrice,tip,tax):
    total = mealPrice + tip + tax
    return total

#this function will print tip, tax, the mealprice, and #the total
def print_info(mealPrice,tip,tax,total):
    print ("The meal price is $",mealPrice)
    print ("The tip is $",tip)
    print ("The tax is $",tax)
    print ("The total is $",total)
    
    
#calls main
main()
