- It says the class/method should have one reason to change.
- It must have only one responsibility.

```
public class Invoice
{
            public void AddInvoice()
            { 
                // your logic
            }

            public void DeleteInvoice()
            { 
                // your logic
            }

            public void GenerateReport()
            { 
                // your logic
            }

            public void EmailReport()
            { 
                // your logic
            }
}

```

- This class can be reconstructed by joining methods **AddInvoice() and DeleteInvoice()** into single class Invoice as they do a similar kind of functionality.
- We will be creating separate classes Report and Email for methods **GenerateReport() and EmailReport()** respectively as they are completely independent and have different functionality. 

```
public class Invoice
{
            public void AddInvoice()
            {
                // your logic
            }

            public void DeleteInvoice()
            {
                // your logic
            }
}

public class Report
{

            public void GenerateReport()
            {
                // your logic
            }
}

public class Email
{
            public void EmailReport()
            {
                // your logic
            }
}

```
