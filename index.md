# The Inner Join
- Selects records from two tables that hold **matching values**
  - Records that don’t hold matching values are excluded from the output
- The query compares each row of the first table with rows of the second table to find rows that satisfy the condition


# Example:

## Here are two tables, Orders and Customers

![Image](/orders.png)

![Image](/customers.png)


## The **SELECT** statement below shows which columns between the two tables are going to be included in the output.
```
SELECT Orders.OrderID, Customers.CustomerName, Orders.OrderDate
```

![Image](/pic1.png)

![Image](/pic2.png)


## Records from both tables that hold matching values are highlighted:
```
FROM Orders INNER JOIN Customers ON Orders.CustID=Customers.CustID;
```
![Image](https://lh3.googleusercontent.com/n7FLlmq-FYZ_0NJFpJxkuIQSe6xdhBE0E9n-pkVL7Nn0g-3YSKgqQdekENOOOSjDiX4Q6lwtXJrSLcJgnonovjhoyYUSuUOodpJE-B7IVbpL5Z45JsRZP-39_nGoT_iijY4EXEfzAsUGYOjAtSMJaoL7UbHRt20oldctNAF5ulC10JL_RZicxcFbFymwZk8x2azoT2s_EILZjzmicGykuYaNgXm6-pmBhPEbwpyvNVjotADRts0lw7NBei1nPpew-9X8n2n_LgsLBvs97E_SrRZ4m3Vtx_3rXWfRp6R6T1Zul7EjtaY4Q00fxjgN41imlupDnqgO4PS0vOdnYSyiT-sPexNNAYQ0A8zDbQRwaYvULvtx13fZR80uyZ14BhKxjvSJqnlVN7dD9o5pZ4_ViIxd7c_xXP7sqFfqnwKcTj_twLXmu2M9Zj9OaFsMkxM2hLxrRmkUuXzNs-8-rcND9RNGaqc_oHfHhYbCzxiyCt8yBMWmZusMQBGGBOpvdxhF7BEWPVuofB5E575t8jwPUETcqrocSPlELn0K1TQB3UfpetWZVqx62sWLrINlY3d5kkY4DkZnn9tqAJMh2RjgfLmWD2yhIN-jwdD7SB2J7dYtFOtNgeztpAhpAOlskAUbeNkIB57Eyq-nImpdqaRw1mnK0pouPwCI=w1284-h157-no)


## The result of the following statement...
```
SELECT Orders.OrderID, Customers.CustomerName, Orders.OrderDate 
FROM Orders INNER JOIN Customers ON Orders.CustID=Customers.CustID;
```
## ...is shown below:
![Image](https://lh3.googleusercontent.com/d0RjDNLbSjRj4mapA_GXRVi88Xn51rzVuAj3-EkBCNNosTnvHqm8k8kqoZipOrEGCLQKoUj7JnyLE0vGt73Jiz1X-QShoc2pnXqsGShVegPphTyPxvNb-5zOCc7Bfj8YwQDo5XvNLBBTbs0TAxdfPF3N4HXswg7flanzLXjkljawCsvjZmD9N1ttY6gtvjeiMgmNZo0TGX9JRjA4PDPpNiG8hjtUQJYEDY1ZCPffVlKhIud-5Y8yGYunleNj5-lZU_GmNN20ph_inpb8NrChf9O0ujmH3bILcVCYw1diSPfsV3ve6JxOBumvht4VfSGT8iiz1pM5YBYxMMDhDo9_5mGiPNtaJjMGD0-BtHIZcSVkYayfdJtGtn5UmHVZt0yoH1D8--v4LeOghhrQZDkGWbLwg6v4MiSPZkfG5sTU6-NCxSH1ncc_GwdnVbQWWD2biiIkdNSewes-loRb5YAMJbG4nSIMQvsTlQEz__tV-aPxQ6Y7b40nGGzhIiYJ9eE4mHK3oDWFnvNFVY1RGR4rqcMSShGP5dwzncfMARSXM0876T6olsLfeylH18Ns2k3b7i0VXA6GMRqS_fUF47RN_IRC_21tlcNR8UU13ah1deYHSMlEm96kFnbVHX1fCX9JojZuDi6WIQmJF3w7OXQNoA9P0G6qOEsk=w1090-h160-no)

