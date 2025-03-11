# Pseudocode

```
START
  PRINT "Enter the total bill amount"
  INPUT bill_amt
  IF (validate(bill_amt)==true)
      PRINT "Quality of service received (poor, fair, good, or excellent)"
      INPUT s_q
      IF (validate_service(s_q)==true)
        PRINT "Number of people splitting the bill"
        INPUT n
        IF (validate(n)==true)
          PRINT "Bill amount:",bill_amt
          PRINT "Service quality:",s_q
          tip_amt=tip(bill_amt,s_q)
          PRINT "Tip amount: ",tip_amt
          total=tip_amt+bill_amt
          PRINT "Total amount: ",total
          PRINT "Number of people:" ,n
          PRINT "Amount per person:",(total/n)
        ELSE
          PRINT "Enter valid number"
      ELSE
        PRINT "Not one of the mentioned ratings"
  ELSE
      PRINT "Enter valid amount"
END

validate(value)
  IF value > 0
    RETURN true
  ELSE
    RETURN false

validate_service(s_q)
  CASE(s_q)
    CASE "poor" : RETURN true
    CASE "fair" : RETURN true
    CASE "good" : RETURN true
    CASE "excellent" : RETURN true
    DEFAULT : RETURN false
  END CASE

tip(bill_amt,s_q)
  CASE(s_q)
    CASE "poor" : RETURN bill_amt*0.10
    CASE "fair" : RETURN bill_amt*0.15
    CASE "good" : RETURN bill_amt*0.18
    CASE "excellent" : RETURN bill_amt*0.20
  END CASE
```
  
    
