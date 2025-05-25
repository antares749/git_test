def main():
    # Get the principal amount
    try:
        principal = float(input("Enter the principal amount: "))
    except ValueError:
        print("The value must be a number!")
        return
    if principal <= 0:
        print("Principal must be positive!")
        return

    
    # Get the annual interest rate
    try:
        annual_rate = float(input("Enter the annual interest rate (in %): "))
    except ValueError:
        print("The value must be a percentage!")
        return
    
    # Get the number of years
    try:
        years = int(input("Enter the number of years: "))
    except ValueError:
        print("The value must be a whoel number!")
        return
    
    # Calculate monthly interest rate
    monthly_rate = annual_rate / 100 / 12
    
    # Calculate number of payments
    num_payments = years * 12
    if annual_rate <= 0:
        monthly_payment = principal / num_payments
    
    # Calculate monthly payment using the formula
    else:
        monthly_payment = principal * (monthly_rate * (1 + monthly_rate) ** num_payments) / ((1 + monthly_rate) ** num_payments - 1)
    
    total_paid = monthly_payment * num_payments
    total_interest = total_paid - principal
    print(f"Total interest paid: ${total_interest:.2f}")
    print(f"The monthly payment is: ${monthly_payment:.2f}")


main()
