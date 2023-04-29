> Total number of clients sales

```1 T number of clients - Sales = COUNT('Marketing - Sales Report'[NAME OF CLIENT])```

> Total number of clients cash
      2 T number of clients - Cash = COUNT('Marketing  Cash Received'[NAME OF CLIENT])

Sum of printing 
      3 Cash Printing Sum = SUM('Marketing  Cash Received'[PRINTING])
Sum of rental 
      4 Cash Rental Sum = SUM('Marketing  Cash Received'[RENTAL])
Sum of sales
      5 Sales Sum = SUM('Marketing - Sales Report'[Sum of CONTRACT SUM])

number of renewals
      6. Count of Renewal = COUNTX('Marketing - Sales Report', 'Marketing - Sales Report'[REMARKS] == "Renewal")
number of new
      7. Count of New = COUNTX('Marketing - Sales Report', 'Marketing - Sales Report'[REMARKS] == "New")

Max money
      8. Max Rental money = MAX('Marketing  Cash Received'[RENTAL])
Average money
     9. Ave Rental Money = AVERAGE('Marketing  Cash Received'[RENTAL])
min money
    9a Min Rental Money = MIN('Marketing  Cash Received'[RENTAL])
