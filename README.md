# Perfect pets
Perfect pets provides private health care for domestic pets throughout the US. This service is provided through various clinics located in the main cities of the US. The director of PerfectPets is concerned that there is a lack of communication within the practice and particularly in the sharing of information and resources across the various clinics. To resolve this problem the director has requested the creation of a centralized database system to assist in the more effective and efficient running of the practice. 

_______________
# Requirements:

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
T123 Penicillin antibiotic course $50.00
T155 Feline hysterectomy $200.00
T112 Vaccination course against feline flu $70.00
T56 Small dog – stay in pen per day (includes feeding) $20.00
A standard rate of $20.00 is charged for each examination, which is recorded
as a type of treatment. The treatment number uniquely identifies each type of
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
