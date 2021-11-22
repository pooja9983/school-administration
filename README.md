# school-administration
import csv
defwrite_into_csv(info_list):
    with open('student_info.csv','a',newline='') as csv_file:
        writer = csv.writer(csv_file)
        
        if csv_file.tell == 0:
           writer.writerow(["name","age","contact number","email id"])
           
           writer.writerow(info_list)

condtion=True

while(condition):
      import student_info=("enter student information in the following  format (name age contact_number email id: ")
       print ("entered information:" +student_info)
     
       student_info_list = student_info.split('')
       print("entered split  up information is:" +str(student_info_list))
      
      write_into_csv(student_info_list)
      
      condition_check=input("enter(yes,no)if you want to enter information for another student:")
        if condition_check=="yes":
            condition = True
        elseif condition_check=="no":
            condition = False
     
