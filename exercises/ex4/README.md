# Internal Orders

In this exercise, you will...
<br>![](/exercises/ex4/images/InternalOrders.png)

## Create Employee Dimension

<br>![](/exercises/ex4/images/create_employee_dimension_02.png)
<br>![](/exercises/ex4/images/create_employee_dimension_03.png)
<br>![](/exercises/ex4/images/create_employee_dimension_10.png)
<br>![](/exercises/ex4/images/create_employee_dimension_04.png)
<br>![](/exercises/ex4/images/create_employee_dimension_05.png)
<br>![](/exercises/ex4/images/create_employee_dimension_06.png)
<br>![](/exercises/ex4/images/create_employee_dimension_07.png)
<br>![](/exercises/ex4/images/create_employee_dimension_08.png)
<br>![](/exercises/ex4/images/create_employee_dimension_09.png)







After completing these steps you will have....

1.	Click here.
<br>![](/exercises/ex0/images/00_00_0010.png)

2.	Insert this code.
```
 DATA(lt_params) = request->get_form_fields(  ).
 READ TABLE lt_params REFERENCE INTO DATA(lr_params) WITH KEY name = 'cmd'.
  IF sy-subrc <> 0.
    response->set_status( i_code = 400
                     i_reason = 'Bad request').
    RETURN.
  ENDIF.
```

## Summary

Now that you have ... 
Continue to - [Exercise 1 - Exercise 1 Description](../ex1/README.md)

