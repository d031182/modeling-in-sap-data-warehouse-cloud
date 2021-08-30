# Sales Orders

In this exercise, you will...

## Level 2 Heading

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

## Generate Time Dimension
1. Navigate to the Space Management
2. Select the section <b><i>Time Data</i></b>.
3. Click on <b><i>Create Time Tables and Dimensions</i></b>
  <br>![](/exercises/ex3/images/create_time_dimension_01.png)
4. The dialog <b><i>Time Table Settings</i><b> will show up.
5. Keep all the default settings and click on <b><i>Create</i></b>
 
<br>![](/exercises/ex3/images/create_time_dimension_02.png)



fefefe
1
2
3
4
5
<br>
<br>
<br>
6
7
<br>
<br>
<br>
<br>
<br>
<br>
7
8
8
u78
87
867
8

8
67
867
6
<br><br>
<br>
<br>
<br>
<br>
7
867
867
867

<br>
<br>
<br>
<br>
867
867
867
867

867
## Level 3 Heading
213232

3

## Summary

Now that you have ... 
Continue to - [Exercise 1 - Exercise 1 Description](../ex1/README.md)
