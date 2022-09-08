# Datebase
Lab1:
1)select * from subject;

2)select count(*) from student;

3)select * from student where student.FIO like 'Ива%';

4)select * from student where student.date_of_birth >= STR_TO_DATE('20051105', '%Y%m%d');

5)select * from student join scores on scores.student = student.FIO 
where scores.score = 4 and scores.subject = 'dsp';

6)select * from student 
join scores on scores.student = student.FIO
join subject on subject.title = scores.subject
where scores.score >= 4  and subject.title = 'dsp'
order by student.FIO
