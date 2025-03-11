# Pseudocode

```
START
  PRINT "Enter the total bill amount"
  INPUT bill_amt
  IF (validate(bill_amt)==true)
      PRINT "How the service quality (poor,fair,good or excellent)"
      INPUT s_q
      IF (check(s_q)==true)
        PRINT "Number of people"
        INPUT n
        IF (validate(n)==true)
          
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
