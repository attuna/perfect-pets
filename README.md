# Perfect pets
Perfect pets provides private health care for domestic pets throughout the US. This service is provided through various clinics located in the main cities of the US. The director of PerfectPets is concerned that there is a lack of communication within the practice and particularly in the sharing of information and resources across the various clinics. To resolve this problem the director has requested the creation of a centralized database system to assist in the more effective and efficient running of the practice. 

__________________
![My Remote Image](https://static01.nyt.com/images/2016/08/05/us/05onfire1_xp/05onfire1_xp-superJumbo-v2.jpg?quality=75&auto=webp)

_______________
# Data requirements:



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
- T56 Small dog – stay in pen per day (includes feeding) $20.00 

*A standard rate of **$20.00** is charged for each examination, which is recorded
as a type of treatment*. The treatment number uniquely identifies each type of
treatment and is used by all PerfectPets clinics.

## Pet treatments
Based on the results of the examination of a sick pet, the vet may propose one
or more types of treatment. For each type of treatment, the information
recorded includes the examination number and date, the pet number, name
and type, treatment number, description, quantity of each type of treatment,
and date the treatment is to begin and end. Any additional comments on the
provision of each type of treatment are also recorded.


## Pens
In some cases, it’s necessary for a sick pet to be admitted to the clinic. Each
clinic has 20–30 animal pens, each capable of holding between one and four
pets. Each pen has a unique pen number, capacity, and status (an indication of
availability). The sick pet is allocated to a pen and the details of the pet, any
treatment(s) required by the pet, and any additional comments about the care
of the pet are recorded. The details of the pet’s stay in the pen are also noted,
which include a pen number, and the date the pet was put into and taken out
of the pen. Depending on the pet’s illness, there may be more than one pet in a
pen at the same time. The pen number is unique to a particular clinic.

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


## Appointments
If the pet requires to be seen by the vet at a later date, the owner and pet are
given an appointment. The details of an appointment are recorded and include
an appointment number, owner number, owner name (first name and last
name), home telephone number, the pet number, pet name, type of pet, and
the appointment date and time. The appointment number is unique to a particular clinic


_________________

# Entities 

- Clinic
- Staff
- PetOwner
- Pet
- Examination
- Treatment
- Pen 
- PetTreatment
- Invoice 
- Appointment
- Stock (with specializations Surgical, NonSurgical, and Pharmaceuticals)


______________________
# Requirements: 

1. **Compulsory functional requirements:**
   - User Authorization
   - User Management (CRUD)
   - Role System
   - Logging

2. **The database should be capable of supporting the following maintenance
transactions:**
   - Create and maintain records recording the details of PerfectPets clinics
and the members of staff at each clinic.
   - Create and maintain records recording the details of pet owners.
   - Create and maintain the details of pets.
   - Create and maintain records recording the details of the types of treatments available for pets.
   - Create and maintain records recording the details of examinations and
treatments given to pets.
   - Create and maintain records recording the details of invoices to pet
   owners for treatment to their pets.
   - Create and maintain records recording the details of surgical, non-surgical, and pharmaceutical supplies at each clinic.
   - Create and maintain records recording the details of pens available at
   each clinic and the allocation of pets to pens.
   - Create and maintain pet owner/pet appointments at each clinic.

3. **The database should be capable of supporting the following example query
transactions:**
   - Present a report listing the Manager’s name, clinic address, and telephone number for each clinic, ordered by clinic number.
   - Present a report listing the names and owner numbers of pet owners
   with the details of their pets.
   - List the historic details of examinations for a given pet.
   - List the details of the treatments provided to a pet based on the results
   of a given examination.
   - List the details of an unpaid invoice for a given pet owner.
   - List the details of pens available on a given date for clinics in New York,
   ordered by clinic number.
   - Present a report that provides the total monthly salary for staff at each
   clinic, ordered by clinic number.
   - List the maximum, minimum, and average cost for treatments.
   - List the total number of pets in each pet type, ordered by pet type.
   - List the appointments for a given date and for a particular clinic.
   - List the total number of pens in each clinic, ordered by clinic number.
   - List the pet number, name, and description of pets owned by a particular owner.
   - Present a report listing the pharmaceutical supplies that need to be
   reordered at each clinic, ordered by clinic number.
_______________
# Database Design
![image](https://user-images.githubusercontent.com/93200268/189105002-7d5a07c5-8747-4dea-8a82-3c62dc73f68f.png)
______________

# Attributes associated with entities:

|Entity|   Attributes|
| ---------- | ----------|
|Clinic |clinicNo, address (street, city, state, zipCode), telNo, faxNo|
|Staff |staffNo, sName (sFName, sLName), sAddress (sStreet, sCity, sState, sZipCode), sTelNo, DOB, sex, SSN, position, salary|
|PetOwner |ownerNo, oName (oFName, oLName), oAddress (oStreet, oCity, oState, oZipCode), oTelNo|
|Pet |petNo, petName, petType, petDescription, pDOB, dateRegistered, petStatus|
|Examination |examNo, examDate, examTime, examResults|
|Treatment |treatNo, description, cost|
|Pen |penNo, penCapacity, penStatus|
|Invoice |invoiceNo, invoiceDate, datePaid, paymentMethod|
|Stock: Item| itemNo, itemName, itemDescription, itemCost|
|Stock: Pharmacy| drugNo, drugName, drugDescription, dosage, methodAdmin, drugCost|
|Appointment |appNo, aDate, aTime|


# Entities

**Clinic**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| clinicNo |integer value, NOT NULL |__Primary Key__|
| street   |variable length character string, NOT NULL|
| city     |variable length character string, NOT NULL|
| state   | variable length character string, NOT NULL| Enumerated Type?|
| zipcode  |fixed length character string length 10, NOT NULL| XXXXX-YYYY, Alternate Key |
| telNo    |fixed length character string length 13, NOT NULL |+1 (three-digit area code) XXX-XXXX, Alternate Key|
| faxNo    |variable length character string| Alternate Key|
| mgrStaffNo   |integer value | __Foreign Key references Staff(staffNo)__|

**Staff** 

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| staffNo | integer value, NOT NULL |__Primary Key__|
| sFName   |variable length character string, NOT NULL|
| sLName     |variable length character string, NOT NULL|
| sCity   |variable length character string, NOT NULL|
| sState   | variable length character string, NOT NULL| Enumerated Type?|
| sZipCode  |fixed length character string length 10, NOT NULL| XXXXX-YYYY|
| sTelNo    |fixed length character string length 13, NOT NULL |+1 (three-digit area code) XXX-XXXX, Alternate Key|
| DOB   |date, NOT NULL|
| SSN    |integer value, NOT NULL| Alternate Key|
| position     |variable length character string, NOT NULL|
| salary     |integer value, >0 |
| clinicNo   |integer value | __Foreign Key references Clinic(clinicNo)__|

**Examination**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| examNo |integer value, NOT NULL |__Primary Key__|
| examDate   |date, NOT NULL|
| examTime     |time, NOT NULL | 
| examResults   | variable length character string, NOT NULL|
| petNo   | integer value, NOT NULL | __Foreign Key references Pet(petNo)__|
| staffNo   | integer value, NOT NULL | __Foreign Key references Staff(staffNo)__|


**PetOwner**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| ownerNo |integer value, NOT NULL |__Primary Key__|
| oFName   |variable length character string, NOT NULL|
| oLName     |variable length character string, NOT NULL|
| oState   | variable length character string, NOT NULL| Enumerated Type?|
| zipcode  |fixed length character string length 10, NOT NULL| XXXXX-YYYY|
| oTelNo    |fixed length character string length 13, NOT NULL |+1 (three-digit area code) XXX-XXXX|
| clinicNo   |integer value, NOT NULL| __Foreign Key references Clinic(clinicNo)__|



**Pet**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| petNo |integer value, NOT NULL |__Primary Key__|
| petName   |variable length character string, NOT NULL|
| petType     |variable length character string, NOT NULL|
| petDescription   | variable length character string, NOT NULL|
| pDOB   |date, NOT NULL|
| dateRegistered   |date, NOT NULL|
| petStatus|  boolean | indicating whether pen is healthy (1) or sick (0)|
| clinicNo   |integer value, NOT NULL| __Foreign Key references Clinic(clinicNo)__|
| ownerNo   |integer value, NOT NULL| __Foreign Key references Owner(ownerNo)__|


**Treatment**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| treatNo |integer value, NOT NULL |__Primary Key__|
| description   |variable length character string, NOT NULL|
| cost      |integer value, >0 |



**Pen**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| penNo |integer value, NOT NULL |__Primary Key__|
| penCapacity   |integer value, NOT NULL, DEFAULT 2, >=1 and <=4|
| penStatus     | boolean | indicating whether pen is available (1) or not available (0)|
| clinicNo   |integer value, NOT NULL| __Foreign Key references Clinic(clinicNo)__|


**Pharmacy**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| drugNo |integer value, NOT NULL |__Primary Key__|
| drugName   |variable length character string, NOT NULL|
| drugDescription   | variable length character string, NOT NULL|
| dosage   | variable length character string, NOT NULL|
| methodAdmin|  boolean | on prescription (1) or without (0)|
| drugCost |integer value, >0 |


**Item**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| itemNo |integer value, NOT NULL |__Primary Key__|
| itemName   |variable length character string, NOT NULL|
| itemDescription   | variable length character string, NOT NULL|
| itemCost  |integer value, >0 |


**Appointment**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| appNo |integer value, NOT NULL |__Primary Key__|
| aDate   |date, NOT NULL|
| aTime   |time, NOT NULL|
| clinicNo   |integer value, NOT NULL| __Foreign Key references Pet(petNo)__|


**Invoice**

|   Column         |   Description   |   Additional info      | 
| ---------------- | ------------- | ------------- |
| invoiceNo |integer value, NOT NULL |__Primary Key__|
| invoiceDate   |date, NOT NULL|
| datePaid   |date, NOT NULL|
| paymentMethod   | variable length character string, NOT NULL| Enumerated Type?|
| examNo   |integer value, NOT NULL| __Foreign Key references Examination(examNo)__|
| ownerNo   |integer value, NOT NULL| __Foreign Key references Owner(ownerNo)__|




