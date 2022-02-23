Welcome to Holy Monkey Memorial Hospital! This softwawre module uses Python and SQLite to create a schedulling application for patients and surgeons. Use this file to track your tasks and any changes.

Thursday 24 February
:: __db__.py
:: __mx__.py
:: __tx__.py (template)

CREATE cursor as **e**

NEW TABLE [patients] and assign PRIMARY KEY and UNIQUE and DATA TYPES
			patientID txt NOT NULL,
			patientForename text,
			patientSurname text,
			patientDateOfBirth text,
			patientGender text,
			patientBloodType text,
			patientMedicare integer,
			patientDonor text,

			UNIQUE (patientID)
			PRIMARY KEY (patientID)

NEW TABLE [items] and assign PRIMARY KEY and UNIQUE and DATA TYPES
			itemID text NOT NULL,
			itemCode text,
			itemCost real,
			itemRebate text,
			itemSupportCategory text,
			
			UNIQUE (itemID)
			PRIMARY KEY (itemID)

NEW TABLE [surgeons] and assign PRIMARY KEY and UNIQUE and DATA TYPES
			surgeonID text NOT NULL,
			surgeonForename text,
			surgeonSurname text,
			surgeonType text,
			surgeonTypeCode text,
			surgeonRegistration text,
			
			UNIQUE (surgeonID)
			PRIMARY KEY (surgeonID)

ASSIGN IF NOT EXISTS

NEW DATA from patient
NEW DATA from item
NEW DATA from surgeons

TEST

**PULL REQUEST :: TASK A :: BRANCH:SQL**
