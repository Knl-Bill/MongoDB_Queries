**A sample data for the queries to run over. 
The "insertMany" function lets us insert an array of documents into the collection**



db.student.insertMany([

{"SRN":"CS21B1001", "Sname": "Alligator", "Degree": "BTech", "Sem": 5, CGPA: 8.01},

{"SRN":"CS21B1002", "Sname": "Crocodile", "Degree": "BTech", "Sem": 6, CGPA: 9.01}, 

{"SRN":"CS21B1003", "Sname": "Bettle", "Degree": "BTech", "Sem": 5, CGPA: 8.51}, 

{"SRN":"CS21M1001", "Sname": "Cricket", "Degree": "MTech", "Sem": 1, CGPA: 8.19}, 

{"SRN":"CS21M1002", "Sname": "Butterfly", "Degree": "MTech", "Sem": 2, CGPA: 6.81}, 

{"SRN":"CS21B1004", "Sname": "Hornet", "Degree": "BTech", "Sem": 6, CGPA: 7.89}, 

{"SRN":"CS21S1001", "Sname": "HoneyBee", "Degree": "BSc", "Sem": 2, CGPA: 7.91}, 

{"SRN":"CS21S1002", "Sname": "Spider", "Degree": "BSc", "Sem": 2, "CGPA": 7.71}, 

{"SRN":"CS21D1001", "Sname": "Blue", "Degree": "Phd", "Sem": 1, CGPA: 8.01}, 

{"SRN":"CS21B1002", "Sname": "Green", "Degree": "Phd", "Sem": 1, CGPA: 9.01}

])
