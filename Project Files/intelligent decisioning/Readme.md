This repository contains the assets for SAS Intelligent Decisioning.

- Lookup Tables
	* Contains the Insurance Base Rate Table along with all the other parameters of Rate Table (RTO, Make, CC, Car etc.). Change the rate values as per your demo requirements.
	* We also created areas where Zaply would not like to insure the P&C product. For the same we created Decline lookup for Make and RTO Location 

- Rule sets
	* Insurance underwriter need flexibility and UI based solution to create and deploy the rules in a governed and secure environment for the same we have created certain rules around eligibility for Fixed and Flexi rules. 
	* With the base rate and rate table (lookup table) we caculated the pure premium for underwriters which is further used in decision (as input for model and discounts)
	* Rules sets are created around offers 

- Treatments
	* Offers created for various decisions

- Decisions
	* 4 Decisions are created to showcase the insurance use cases
		* Fixed and Flexi decisions are made for customer acquisitions 
		* Add on decision created for mobile webapp based on terrain, travel days and demographic history of the customer
		* Xsell decisioning - this decision includes the python model directly deployed in the decision to showcase Xsell products which are relevant for the customer

All the relevant CSV's and documentation are uploaded 