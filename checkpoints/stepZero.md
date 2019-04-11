
# Pre work

In challenge crucial part of code is to avoid loading whole tree structure into memory. To understand this,
start to train example with infinite iteration which force you to avoid loading "everything" into memory
Example: Let's consider cyclic meetings in every Tuesday and Friday. We know only starting date (e.g. 2016/IX/19)
and we would like to go enumerate calendar days.
Create fully tested class called Calendar which is Iterable<LocalDate> and prove that.
<br /><br />

- You can initialize Calendar 2016/IX/19 as the LocalDate instance, and you can obtain 2016/IX/20,
2016/IX/23, 2016/IX/27, 2016/IX/30 as initial to keep clean code, instead of 'manually' checking every returned
value use collections assert available in either Assertj or Hamcrest.
- Calendar can produce independent iterators - using the first ne doesn't have an impact on the second one iteration
<br /><br />

**Tips**<br />
Review iterable / iterator documentation