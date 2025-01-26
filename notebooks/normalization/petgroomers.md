| Appointment ID | Pet Owner Name | Contact Info         | Appointment Date  | Services Requested                       | Products Used           | Total Cost | Tip Amount |
| -------------- | -------------- | -------------------- | ----------------- | ---------------------------------------- | ----------------------- | ---------- | ---------- |
| A9001          | Olivia Green   | olivia.g@example.com | 2024-09-01        | "Bath", "Haircut"                        | Shampoo, Conditioner    | $45.00     | 1          |
| A9002          | Ethan Hunt     | (555) 654-3210       | 09/02/2024        | "Nail Trimming"                          | Nail Clippers           | 15.00      | $5         |
| A9003          | Ava Brown      | ava.b@domain.com     | September 3, 2024 | "Bath", "Ear Cleaning", "Teeth Brushing" | Ear Cleaner, Toothpaste | $60        | Ten Bucks  |
| A9004          | Liam Smith     | liam.smith@abc.net   | 2024/09/04        | "Haircut"                                | Scissors                | $25.00     | None       |
| A9005          | Olivia Green   | olivia.g@example.com | 09-05-2024        | "Bath"                                   | Shampoo                 | 20.00      | A cookie   |
| A9006          | Mia Johnson    | 555-789-0123         | 2024-09-06        | "Haircut", "Nail Trimming"               | Scissors, Nail Clippers | $35.75     | $10        |


## 1NF
| Appt. Id | Owner Name | Email | Phone Number | Appt. Date | Services | Products | Total | Tip |
| -------- | ---------- | ----- | ------------ | ---------- | -------- | -------- | ----- | --- |

### Data Types 
- Appt. Id: integer 
- Owner Name: string
- Email: string 
- Phone Number: integer
- Appt. Date: date-time 
- Services: string
- Products: string 
- Total: money 
- Tip: money

### PK
- Appt. Id

### No Repeating groups

| Appointment ID | Pet Owner Name | Contact Info         | Appointment Date  | Services Requested                       | Products Used           | Total Cost | Tip Amount |
| -------------- | -------------- | -------------------- | ----------------- | ---------------------------------------- | ----------------------- | ---------- | ---------- |
| A9001          | Olivia Green   | olivia.g@example.com | 2024-09-01        | "Bath"                                   | Shampoo, Conditioner    | $45.00     | 1          |
| A9001          | Olivia Green   | olivia.g@example.com | 2024-09-01        | "Haircut"                                | Shampoo, Conditioner    | $45.00     | 1          |
| A9002          | Ethan Hunt     | (555) 654-3210       | 09/02/2024        | "Nail Trimming"                          | Nail Clippers           | 15.00      | $5         |
| A9003          | Ava Brown      | ava.b@domain.com     | September 3, 2024 | "Bath", "Ear Cleaning", "Teeth Brushing" | Ear Cleaner, Toothpaste | $60        | Ten Bucks  |
| A9004          | Liam Smith     | liam.smith@abc.net   | 2024/09/04        | "Haircut"                                | Scissors                | $25.00     | None       |
| A9005          | Olivia Green   | olivia.g@example.com | 09-05-2024        | "Bath"                                   | Shampoo                 | 20.00      | A cookie   |
| A9006          | Mia Johnson    | 555-789-0123         | 2024-09-06        | "Haircut", "Nail Trimming"               | Scissors, Nail Clippers | $35.75     | $10        |

- Then would go in and create seprate tables

table one (appt. info)
- Appt. ID
- Owner Name
- Contact Info
- Appt. Date

table two (services)
- Appt. ID
- Services
- Products

then possibly, table three (money)
- Appt. ID
- Total
- Tip

### Dependencies 
- Everything depends on Appt. ID
- 

