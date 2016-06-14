# 注意：

* 错误：

  ~~~ bash
  [helen@zhangyingyun awk]$ awk -v stu_name = Bob 'BEGIN{printf "Name = %s\n", stu_name} {print}' new_stu.txt
  awk: `stu_name' argument to `-v' not in `var=value' form
  ~~~

* 正确：
  ~~~ bash
  [helen@zhangyingyun awk]$ awk -v stu_name=Bob 'BEGIN{printf "Name = %s\n", stu_name} {print}' new_stu.txt
  Name = Bob
  SrNo  stuName  stuSub     stuMark
  1)    Amit     Physics    80
  2)    Rahul    Maths      90
  3)    Shyam    Biology    87
  4)    Kedar    English    85
  5)    Hari     History    89
  ~~~


`stu_name = Bob` 等号两边不能有空格


