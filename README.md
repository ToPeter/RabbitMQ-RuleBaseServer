# RabbitMQ-RuleBaseServer

###How to run


 1. Run project.
 2. Click -> [here](http://localhost:8080/RuleBaseService/RuleBaseService?Tester) <- to run Test web page.
 3. Type data values:
	- String ssn ()
    - int creditScore ()
    - double loanAmount ()
    - Date loanDuration ()

#### Choose Bank Logic

```java
if (creditScore < 580)
      return null;
if (creditScore >= 720)
      get 4 banks as result;
if (creditScore >= 680 && creditScore <= 719)
      get 3 banks as result;
if (creditScore >= 620 && creditScore <= 679)
      get 2 banks as result;
if (creditScore >= 580 && creditScore <= 619)
      get 1 bank;

 return selectedBank as result;
```

#### TODO 
 - are there predefined creditScore Values ?