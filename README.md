# BD-2022-2023
DATABASE MANAGEMENT APPLICATION FOR CLINIC CHAIN - MySQL, Java

__INTRODUCTION__

The project aims to develop an application for managing a network of polyclinics through a database. The purpose of the application is to simplify access to and manipulation of the database through a graphical interface that can be used by employees. The application allows for the creation of appointments for specific medical services by a competent doctor and generates invoices. There are multiple types of users, including administrators and super administrators who have full access to data, and employees who have limited access to data depending on their type. There are also three departments dealing with human resources, financial and accounting aspects, and medical aspects. The project objectives are to streamline polyclinic operations, compete with operations, ensure data security, avoid tax evasion, and reduce paper and plastic consumption. For the project development, the following tools were used:

-MySQL Workbench 6.2: for creating the database, initial population, development of views, procedures and triggers, and for creating the UML diagram of the tables.

-Eclipse/IntelliJ: Java development environment.

__THE ASSUMPTIONS OF THE POLYCLINIC (REQUIREMENTS AND CONSTRAINTS)__

The application manages the actions of employees within a unit, utilizing a database subject to the following requirements:

-There are 3 types of users: employees, administrators, and super-administrators.

-A user is uniquely identified by their ID number (CNP), for whom we also store their name, surname, address, phone number, email, IBAN account, contract number, hiring date, and the position held within the chain of polyclinics.

-There are multiple medical units within the polyclinic chain, each uniquely identified by name, and additionally containing their address and schedule ID.

-There are multiple types of roles: human resources inspectors, financial experts, receptionists, medical assistants, and doctors.

-For a medical assistant, we additionally retain type and grade.

-For a doctor, we additionally retain their specialty or specialties, grade, identification code, competencies required for special procedures, and academic title. Additionally, each doctor has a negotiated percentage of the medical services performed that they are entitled to, in addition to their negotiated salary.

-The polyclinic chain offers patients a set of specific medical services for each specialty. For each available medical service, the associated specialty, the necessity of the doctor's competency, the associated price, and the duration (expressed in minutes) will be specified.

-The system will consist of multiple modules accessible to employees based on their rights. Thus, modules for:  
__Human resources management__, which includes managing employee schedules and leaves.

__Financial and accounting operations__, determining operational profit as the difference between income (amounts collected for medical services) and expenses (payments made to employees for salaries).

__Operational activity management__, including patient scheduling for medical services, registration upon arrival at the medical clinic, issuance of invoices by receptionists, and completion of medical reports by medical assistants and doctors.
