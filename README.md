# Name=Chandra Prakash Mishra
# Date=12/10/2025
# Project title = Daily Calorie Tracker (CLI)
print("Welcome Sir/Madam to Daily Calorie Tracker Application,this application helps you to track your daily calorie intake and expenditure.This application is designed to help you maintain a healthy lifestyle by monitoring your calorie consumption and physical activities.")
# Features:

# 1. Add Food Intake: Add the food items you consume along with their calorie values.
# displays the total meals conusmed today.
print(" --------------------------------------------------")
Total_meals_list=[]
Total_meals=int(input("Enter the total number of meals you want to add:"))
Total_meals_list=Total_meals
# another option was to do   ----Total_meals_list.append(Total_meals)
# this list will store the meal names.
Meals_list=[]
# this list will store the calorie intake values.
Calories_intake_list=[]
#sum variable to store total calories, which is initialized to 0.
sum=0
# loop to add meals and their calorie intake.
for i in range(Total_meals_list):
    Meals_Name=input("Enter the meal name(Q or q to quit):")
    # append meal name to the Meals_list
    Meals_list.append(Meals_Name)
    # check for quit condition
    if Meals_Name=='Q' or Meals_Name=='q':
        break
    else:
        Calories_intake=(int(input("Enter the calories intake(Q or q to quit):")))
        # append calorie intake to the Calories_intake_list
        Calories_intake_list.append(Calories_intake)
        # check for quit condition
        if Calories_intake=='Q' or Calories_intake=='q':
            break
        else:
         print(f"Meals Name:{Meals_list},Calories Intake:{Calories_intake_list}")
         
    # 2. View Total Calories: View the total calories consumed throughout the day.     
    sum= sum+Calories_intake
    print(f"Total Calories Intake so far:{sum}")
            
# 3. View Daily Summary: Get a summary of your avg calorie intake per meal for the day.
avg=sum/len(Calories_intake_list)
print(f"Average Calories Intake so far:{avg}")
            
# 4. Set Daily Calorie Goal: Set a target for your daily calorie intake.
Calorie_limit=int(input("Enter your daily calorie limit:"))
if sum>Calorie_limit:
    print("Warning: You have exceeded your daily calorie limit!")
else:
     print("congratulations!,You are within your daily calorie limit. Keep it up!")
       
            
        
       
           
         
           
    
    


