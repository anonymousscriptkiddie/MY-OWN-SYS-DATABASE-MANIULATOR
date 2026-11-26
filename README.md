DELETE FROM TODO_LIST;
Insert INTO TODO_LIST( subject, grades, gwa, progress,advancedReview, projects, dueDate, numberOf,Homework, seatwork, quiz)
VALUES ('Object oriented Programming', '9 out of 10', null, 'Finished', 'python', 'null' , 11-28-2026, 1, null, null, 'yes'),
       ('Object oriented Programming', '60 out of 60', null, 'Finished', 'cpp', null, 11-26-2026, 2, 'yes', 'yes', null),
       ('Engineering Data Analysis', 15, null, 'Progressed', 'Statistics', 'null', 11-25-2026, 3, 'no', null, 'yes'),
	   ('Mathematics in the modern world', null, null, 'Progressed', 'Golden Ratio', 'null', 11-25-2026, 4, 'no', 'yes', 'yes'),
	   ('Calculus 2', 5, null, 'Progressed', 'U-substitution', null, 11-25-2026, 5, 'yes', null, 'yes'),
	   ('Pathfit', null, null, 'Progressed', 'Static', 'dynamics',11, 6, 'no', null, null),
	   ('Discrete Mathematics', 1, null, 'Progressed', 'Properties of sets', 'Dream project', 0, 7, null, 'yes', null),
	   ('Physics for engineering', 1, null, 'Progressed', 'Scalar and vector/acceleration', 'object with motion', 0, 8, null, null, null),
	   ('Engineering Data Analysis Laboratory', 'completed', null, 'Finished/Progressed', null, 'certification', 'january', 9, 'yes', 'yes', 'yes');
       
SELECT *FROM TODO_LIST;

DROP TABLE IF EXISTS "Finished";

CREATE TABLE "Finished" AS
SELECT * FROM TODO_LIST
WHERE progress = 'Finished';
SELECT * FROM "Finished";
