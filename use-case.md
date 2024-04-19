mermaid'''
skinparam packageStyle rectangle

actor Accountant
actor Manager

rectangle "Spreadsheet Accounting System" {
  (Record Transaction) as (UC1)
  (Create Account) as (UC2) 
  (Generate Financial Statements) as (UC3)  
  (View Account Details) as (UC4)
}

Accountant --> (UC1)
Accountant --> (UC2)
Accountant --> (UC3)
Accountant --> (UC4)

Manager --> (UC3)
Manager --> (UC4)
'''
