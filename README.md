# Perfect pets by *Hanna Peshko 053501*
Perfect pets provides private health care for domestic pets throughout the US. This service is provided through various clinics located in the main cities of the US. The director of PerfectPets is concerned that there is a lack of communication within the practice and particularly in the sharing of information and resources across the various clinics. To resolve this problem the director has requested the creation of a centralized database system to assist in the more effective and efficient running of the practice. 

__________________
![My Remote Image](https://static01.nyt.com/images/2016/08/05/us/05onfire1_xp/05onfire1_xp-superJumbo-v2.jpg?quality=75&auto=webp)
____________________
 
# Project navigation
![image](https://user-images.githubusercontent.com/93200268/189360910-a74e26c1-90b9-42ec-85f4-fad9331d68bb.png)
___________
# Data requirements


##  Veterinary clinics
PerfectPets has many veterinary clinics located in the main cities of the US. The
details of each clinic include the clinic number, clinic address (consisting of the
street, city, state, and zip code), and the telephone and fax numbers. Each clinic
has a Manager and a number of staff (for example, vets, nurses, secretaries,
cleaners). The clinic number is unique.


## Staff
The details stored on each member of staff include the staff number, name (first
and last), address (street, city, state, and zip code), telephone number, date of
birth, sex, social security number (SSN), position, and current annual salary.
The staff number is unique.

## Pet owners
When a pet owner first contacts a clinic of PerfectPets the details of the pet
owner are recorded, which include an owner number, owner name (first name
and last name), address (street, city, state, and zip code), and home telephone
number. The owner number is unique to a particular clinic. 

## Pets
The details of the pet requiring treatment are noted, which include a pet
number, pet name, type of pet, description, date of birth (if unknown, an
approximate date is recorded), date registered at clinic, current status
(alive/deceased), and the details of the pet owner. The pet number is unique to
a particular clinic.

## Examinations
The details of each examination are recorded and include an examination number,
the date and time of the examination, the name of the vet, the pet number, pet
name, and type of pet, and a full description of the examination results. The
examination number is unique to a particular clinic. As a result of the examination, the vet may propose treatment(s) for the pet.

## Treatments
PerfectPets provides various treatments for all types of pets. These treatments are
provided at a standard rate across all clinics. The details of each treatment
include a treatment number, a full description of the treatment, and the cost to
the pet owner. For example, treatments include:
- T123 Penicillin antibiotic course $50.00
- T155 Feline hysterectomy $200.00
- T112 Vaccination course against feline flu $70.00 
- T56 Small dog – stay in cage per day (includes feeding) $20.00 

*A standard rate of **$20.00** is charged for each examination, which is recorded
as a type of treatment*. The treatment number uniquely identifies each type of
treatment and is used by all PerfectPets clinics.


## Cages
In some cases, it’s necessary for a sick pet to be admitted to the clinic. Each
clinic has 20–30 animal cages, each capable of holding between one and four
pets. Each cage has a unique cage number, capacity, and status (an indication of
availability). The sick pet is allocated to a cage and the details of the pet, any
treatment(s) required by the pet, and any additional comments about the care
of the pet are recorded. The details of the pet’s stay in the cage are also noted,
which include a cage number, and the date the pet was put into and taken out
of the cage. Depending on the pet’s illness, there may be more than one pet in a
cage at the same time. The cage number is unique to a particular clinic.

## Invoices
The pet owner is responsible for the cost of the treatment given to a pet.The
details recorded on the invoice include the invoice number, invoice date, owner
number, owner name and full address, pet number, pet name, and the details of
the treatment given. The invoice provides the cost for each type of treatment
and the total cost of all treatments given to the pet.
Additional data is also recorded on the payment of the invoice, including the
date the invoice was paid and the method of payment (for example, check,
cash, credit card). The invoice number is unique.

## Surgical, non-surgical, and pharmaceutical supplies
Each clinic maintains a stock of surgical supplies (for example, syringes, sterile
dressings, bandages) and non-surgical supplies (for example, plastic bags,
aprons, litter trays, pet name tags, pet food). The details of surgical and nonsurgical supplies include the item number and name, item description, quantity
in stock (this is ascertained on the last day of each month), reorder level,
reorder quantity, and cost. The item number uniquely identifies each type of
surgical or non-surgical supply. The item number is unique for each surgical or
non-surgical item and used throughout the practice. Each clinic also maintains a stock of pharmaceutical supplies (for example,
antibiotics, pain killers). The details of pharmaceutical supplies include a drug
number and name, description, dosage, method of administration, quantity in
stock (this is ascertained on the last day of each month), reorder level, reorder
quantity, and cost. The drug number uniquely identifies each type of pharmaceutical supply. The drug number is unique for each pharmaceutical supply.


__________________
```
Your advertisement
   could be here 
```
_________________


# Entities descripton

- Clinic
- Staff
- PetOwner
- Pet
- Examination
- Treatment
- Cage
- Invoice 
- Stock (with specializations Surgical, NonSurgical, and Pharmaceuticals)

______________________
# Requirements

1. **Compulsory functional requirements:**
   - User Authorization
   - User Management (CRUD)
   - Role System (Admin, Manager, Staff)
   - Logging

2. **The database should be capable of supporting the following maintenance
transactions:**
   - Create and maintain records recording the details of PerfectPets clinics
and the members of staff at each clinic. (Admin)
   - Create and maintain records recording the details of pet owners. (Admin, Manager)
   - Create and maintain the details of pets. (Admin, Manager)
   - Create and maintain records recording the details of the types of treatments available for pets. (Admin, Manger, Staff)
   - Create and maintain records recording the details of examinations and
treatments given to pets.  ( Admin, Manger, Staff)
   - Create and maintain records recording the details of invoices to pet
   owners for treatment to their pets.  ( Admin, Manger, Staff)
   - Create and maintain records recording the details of surgical, non-surgical, and pharmaceutical supplies at each clinic.  ( Admin, Manger, Staff)
   - Create and maintain records recording the details of cages available at
   each clinic and the allocation of pets to cages.  ( Admin, Manger, Staff)

3. **The database should be capable of supporting the following example query
transactions:**
   - Present a report listing the Manager’s name, clinic address, and telephone number for each clinic, ordered by clinic number.
   - Present a report listing the names and owner numbers of pet owners
   with the details of their pets. 
   - List the historic details of examinations for a given pet. 
   - List the details of the treatments provided to a pet based on the results
   of a given examination.
   - List the details of an unpaid invoice for a given pet owner. 
   - List the details of cages available on a given date for clinics in New York,
   ordered by clinic number.
   - Present a report that provides the total monthly salary for staff at each
   clinic, ordered by clinic number.
   - List the maximum, minimum, and average cost for treatments.
   - List the total number of pets in each pet type, ordered by pet type.
   - List the total number of cages in each clinic, ordered by clinic number.
   - List the pet number, name, and description of pets owned by a particular owner.
   - Present a report listing the pharmaceutical supplies that need to be
   reordered at each clinic, ordered by clinic number.
_______________
# Database Design

![image](https://user-images.githubusercontent.com/93200268/189854633-a9cd5279-1fd1-49ab-bea9-24e1826bcbc5.png)



______________

# Attributes associated with entities:

|Entity|   Attributes|
| ---------- | ----------|
|Clinic |id, address (street, city, state, zip_code), tel, fax|
|Staff |id, name (first_name, last_name), address (street, city, state, zip_code), tel, DOB, sex, SSN, position, salary|
|PetOwner |id, name (first_name, last_name), address (street, city, state, zip_code), tel|
|Pet |id, name, type, description, DOB, date_registered, status|
|Examination |id, date, time, results, staff_id, pet_id, treatment_id|
|Treatment |id, description, cost, staff_id|
|Cage |id, capacity, status, pet_id|
|Invoice |id, date, date_paid, payment_method, treatment_id|
|Stock: Item| id, name, description, cost, quantity|
|Stock: Pharmacy| id, name, description, dosage, method_admin, cost, quantity|

_______________
![27f44542-64e5-4b4c-9a30-39fa4fce02e5](https://user-images.githubusercontent.com/93200268/190670094-1c445a69-407e-4956-bc2d-0e082ca0f44c.jpg)

_______________


# Entities

### **Clinic**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| clinic_id |int, NOT NULL |__Primary Key__|
| street   |VARCHAR(50), NOT NULL|
| city     |VARCHAR(50), NOT NULL|
| state   |VARCHAR(50), NOT NULL| Enumerated Type?|
| zip_code  |CHAR(10), NOT NULL| XXXXX-YYYY, Alternate Key |
| tel    |CHAR(13), NOT NULL |+1 (three-digit area code) XXX-XXXX, Alternate Key|
| fax    |VARCHAR(50), NOT NULL| Alternate Key|
| staff   || __Foreign Key references Staff(staff_id)__|

### **Staff** 

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| staff_id |int, NOT NULL |__Primary Key__|
| first_name   |VARCHAR(50), NOT NULL|
| last_name     |VARCHAR(50), NOT NULL|
| city   |VARCHAR(50), NOT NULL|
| street   | VARCHAR(50), NOT NULL| |
| sex   |ENUM('M','W'), NOT NULL| Enumerated Type|
| zip_code  |CHAR(10), NOT NULL| XXXXX-YYYY|
| tel    |CHAR(13), NOT NULL |+1 (three-digit area code) XXX-XXXX, Alternate Key|
| DOB   |DATE, NOT NULL|
| SSN    |CHAR(6), NOT NULL| Alternate Key|
| position     |VARCHAR(50), NOT NULL|
| salary     |int,>0, NOT NULL  |
| clinic   | | __Foreign Key references Clinic(clinic_id)__|
| role | ENUM ("Admin", "Manager", "Stuff"), NOT NULL| | 

### **Examination**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| exam_id |int, NOT NULL |__Primary Key__|
| date   |DATE, NOT NULL|
| time     |TIME, NOT NULL | 
| results   | VARCHAR(500), NOT NULL|
| pet   | | __Foreign Key references Pet(pet_id)__|
| staff   | | __Foreign Key references Staff(staff_id)__|


### **PetOwner**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| owner_id |serial, NOT NULL |__Primary Key__|
| first_name   | VARCHAR(50), NOT NULL|
| last_name     | VARCHAR(50), NOT NULL|
| state   |  VARCHAR(50), NOT NULL| Enumerated Type?|
| zip_code  |CHAR(10), NOT NULL| XXXXX-YYYY|
| tel    |CHAR(13), NOT NULL |+1 (three-digit area code) XXX-XXXX, Alternate Key|
| clinic   | | __Foreign Key references Clinic(clinic_id)__|


### **Pet**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| pet_id |serial, NOT NULL |__Primary Key__|
| name   |VARCHAR(50), NOT NULL|
| type     |VARCHAR(50), NOT NULL|
| description   | VARCHAR(150)|
| DOB   |DATE, NOT NULL|
| date_registered   |DATE, NOT NULL|
| status|  BOOLEAN, NOT NULL| indicating whether pet is healthy (1) or sick (0), default H|
| clinic   || __Foreign Key references Clinic(clinic_id)__|
| owner   || __Foreign Key references Owner(owner_id)__|


### **Treatment**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| tratment_id |serial, NOT NULL |__Primary Key__|
| description   |VARCHAR(1500), NOT NULL|
| cost      |integer, >0, NOT NULL|




### **Cage**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| cage_id |serial, NOT NULL |__Primary Key__|
| capacity   |integer, NOT NULL, DEFAULT 2, >=1 and <=4|
| status     | BOOLEAN, NOT NULL | indicating whether cage is available (1) or not available (0), default A|
| clinic   || __Foreign Key references Clinic(clinic_id)__|
| clinic   || __Foreign Key references Clinic(clinic_id)__|



### **Pharmacy**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| pharmacy_id |serial, NOT NULL |__Primary Key__|
| name   |VARCHAR(50), NOT NULL|
| description   | VARCHAR(1500), NOT NULL |
| dosage   | VARCHAR(150), NOT NULL|
| on_prescription|  BOOLEAN, NOT NULL |	indicating whether drug is available on prescription (1) or without (0)|
| cost |integer, >0, NOT NULL|
| clinic   || __Foreign Key references Clinic(clinic_id)__|


### **Item**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| item_id |serial, NOT NULL |__Primary Key__|
| name   |VARCHAR(50), NOT NULL|
| description   | VARCHAR(1500), NOT NULL |
| cost |integer, >0, NOT NULL|
|quantity| int, >0, NOT NULL|
| clinic   || __Foreign Key references Clinic(clinic_id)__|



### **Invoice**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| invoice_id |serial, NOT NULL |__Primary Key__|
| date   |DATE, NOT NULL|
| date_paid   |DATE, NOT NULL|
| payment_method   |ENUM ('CARD', 'CASH','CHECK'),  NOT NULL| 
| exam  || __Foreign Key references Examination(exam_id)__|
| owner   || __Foreign Key references Owner(owner_id)__|



_______________

# Normalized tables
_______________


### **Clinic**

| Field         | Type            | Null            | Key              |  Additional info  |
|:------------- |:--------------- |:--------------- |:---------------  |:--------------- |
| id | INT  | NOT NULL | PRIMARY KEY  | AUTO_INCREMENT |
| address_id | INT | NOT NULL | FOREIGN KEY | UNIQUE |
| contact_id | INT | NOT NULL | FOREIGN KEY | UNIQUE |


### **Staff**

| Field         | Type            | Null            | Key             | Additional info |
|:------------- |:--------------- |:--------------- |:--------------- |:--------------- |
| id | INT    | NOT NULL |  PRIMARY KEY  | AUTO_INCREMENT |
| fullname_id  | INT | NOT NULL | FOREIGN KEY ||
| address_id | INT | NOT NULL | FOREIGN KEY ||
| contact_id | INT | NOT NULL | FOREIGN KEY | UNIQUE |
| sex | ENUM('M', 'W') | NOT NULL |||
| SSN | CHAR(6) | NOT NULL ||UNIQUE |
| position | VARCHAR(50) | NOT NULL |||
| salary | DECIMAL(10, 2) | NOT NULL || >0 |
| clinic_id | INT | NOT NULL | FOREIGN KEY | |
| role | ENUM("Admin", "Manager", "Stuff") | NOT NULL |||

### **Pet**

| Field         | Type            | Null            | Key             | Additional info   |
|:------------- |:--------------- |:--------------- |:---------------  |:--------------- |
| id | INT    | NOT NULL | PRIMARY KEY | AUTO_INCREMENT |
| name  | VARCHAR(50) | NOT NULL |  ||
| address_id | INT | NOT NULL | FOREIGN KEY ||
| sex | ENUM('M', 'W') | NOT NULL |||
| DOB| DATE| NOT NULL| ||
| owner_id|  INT| NOT NULL| FOREIGN KEY ||

### **PetOwner**

| Field         | Type            | Null            | Key             | Additional info   |
|:------------- |:--------------- |:--------------- |:---------------  |:--------------- |
| id | INT    | NOT NULL | PRIMARY KEY || AUTO_INCREMENT |
| fullname_id  | INT |  NOT NULL |  FOREIGN KEY ||
| address_id | INT | NOT NULL |  FOREIGN KEY ||
| contact_id  | INT | NOT NULL |  FOREIGN KEY | |UNIQUE |
| sex | ENUM('M', 'W') | NOT NULL ||
| registration_date | DATE | NOT NULL | | CHECK(registration_date <= CURRENT_DATE)|

### **Examination**

| Field         | Type            | Null            | Key            | Additional info  |
|:------------- |:--------------- |:--------------- |:---------------|:--------------- |
| id | INT  |  NOT NULL | PRIMARY KEY |  AUTO_INCREMENT |
| time | DATETIME | NOT NULL | CHECK(time <= CURRENT_TIME)|
| staff_id | INT |  NOT NULL |FOREIGN KEY||
| pet_id | INT |  NOT NULL |FOREIGN KEY||
| results | TEXT |  NOT NULL ||


### **Treatment**

| Field         | Type            | Null            | Key             | Additional info  |
|:------------- |:--------------- |:--------------- |:--------------- |:--------------- |
| id | INT  | NOT NULL | PRIMARY KEY |  AUTO_INCREMENT |
| description | TEXT | NOT NULL ||
| staff_id | INT | NOT NULL | FOREIGN KEY||
| invoice_id | INT | NOT NULL | FOREIGN KEY| UNIQUE |
| examination_id | INT | NOT NULL | FOREIGN KEY||

### **Cage**

| Field         | Type            | Null            | Key             |  Additional info   |
|:------------- |:--------------- |:--------------- |:--------------- |:--------------- |
| id | INT  | NOT NULL |  PRIMARY KEY  | AUTO_INCREMENT |
| size | ENUM('HEAD', 'SMALL', 'MEDIUM', 'LARGE') | NOT NULL ||
| status |  BOOLEAN| NOT NULL | ||
| pet_id | INT | + | FOREIGN KEY |UNIQUE |
| clinic_id | INT | NOT NULL | FOREIGN KEY | |


### **Invoice**

| Field         | Type            | Null            | Key             | Additional info   |
|:------------- |:--------------- |:--------------- |:---------------  |:--------------- |
| id | INT  | NOT NULL | PRIMARY KEY | NULL | AUTO_INCREMENT |
| date_issue | DATE | NOT NULL || CHECK(date_issue <= CURRENT_DATE)|
| date_paid | DATE | + || CHECK(date_paid <= CURRENT_DATE)|
| cost | DECIMAL(10, 2) | NOT NULL || POSITIVE |
| payment_method | ENUM('CARD', 'CASH', 'CHECK') | + |


### **StockItem**

| Field         | Type            | Null            | Key              | Additional info   |
|:------------- |:--------------- |:--------------- |:---------------  |:--------------- |
| id | INT  |  NOT NULL | PRIMARY KEY |  AUTO_INCREMENT |
| name | VARCHAR(50) |  NOT NULL | UNIQUE |
| description | TEXT |  NOT NULL ||
| cost | DECIMAL(10, 2) |  NOT NULL | POSITIVE |
| quantity | INT |  NOT NULL |  |POSITIVE |
| clinic_id | INT |  NOT NULL | FOREIGN KEY |  |


### **StockPharmacy**

| Field         | Type            | Null            | Key             | Additional info  |
|:------------- |:--------------- |:--------------- |:--------------- |:--------------- |
| id | INT  |  NOT NULL | PRIMARY KEY |  AUTO_INCREMENT |
| name | VARCHAR(50) | NOT NULL || UNIQUE |
| description | TEXT | NOT NULL |||
| dosage | TEXT | NOT NULL |||
| on_prescription | BOOLEAN | NOT NULL ||
| cost | DECIMAL(10, 2) | NOT NULL || POSITIVE |
| quantity | INT | NOT NULL |  | POSITIVE |
| clinic_id | INT | NOT NULL | FOREIGN KEY | |


### **Address**

| Field         | Type            | Null            | Key             | Additional info  |
|:------------- |:--------------- |:--------------- |:---------------  |:--------------- |
| id | INT  |  NOT NULL | PRIMARY KEY |  AUTO_INCREMENT |
| city | VARCHAR(50) |  NOT NULL  |||
| street | VARCHAR(50) |  NOT NULL  |||
| home | VARCHAR(50) |  NOT NULL  |||


### **Fullname**

| Field         | Type            | Null            | Key             | Additional info  |
|:------------- |:--------------- |:--------------- |:---------------  |:--------------- |
| id | INT  |  NOT NULL | PRIMARY KEY |  AUTO_INCREMENT |
| first_name  | VARCHAR(50) | NOT NULL |
| middle_name | VARCHAR(50) | NOT NULL ||
| last_name   | VARCHAR(50) | NOT NULL ||


### **Contact**

| Field         | Type            | Null            | Key             | Additional info  |
|:------------- |:--------------- |:--------------- |:--------------- |:--------------- |
| id | INT  |  NOT NULL | PRIMARY KEY |  AUTO_INCREMENT |
| tel | CHAR(13) | NOT NULL |||
| email | VARCHAR(50) | NOT NULL |||
| fax | VARCHAR(50) | + |||





