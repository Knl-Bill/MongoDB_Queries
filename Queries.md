**1. Display all the documents.**

db.student.find()

**2.  Display all the students in B.Tech.**

db.student.find({Degree: "BTech"})

**3. Display all the students in ascending order**

db.student.find().sort({Sname:1})

**4. Display first 5 students**

db.student.find().limit(5)

**5. Display students 5,6,7**

db.student.find().skip(4).limit(3)

**6. List the degree of a student whose name is “XYZ”. (give any specific name)**

db.student.findOne({Sname: "XYZ"}, {Degree: 1})

**7. Display students details of 5,6,7 in descending order of CGPA**

db.student.find().skip(4).limit(3).sort({CGPA:-1})

**8. Display the number of students in B.Tech**

db.student.countDocuments({Degree: "BTech"})

**9. Display all the degrees without_id**

db.student.find({},{Degree:1, _id:0})

**10. Display the distinct degrees**

db.student.distinct(Degree)

**11. Display all the B. Tech students with CGPA greater than 6, but less than 7.5**

db.student.find({Degree: "BTech", CGPA: {$gt : 6.0, $lt : 7.5}})

**12. Display all the students in B. Tech and in 5th Sem**

db.student.find({Degree: "BTech", Sem: 5})
