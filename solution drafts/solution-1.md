# Solution 1: "SAM"

## Concept Summary

 * Local storage and validation
 * All-in-one-device solution
 * Entirely local in the station
 * Local display and input

 
## Solution description

This solution describes the SAM of EBG Compleo. SAM is a storage and display modul for the meter values, so the user can check his meter values for the required period of time at the chareing station.

 * The module stores start and end reading of the meter for each charging session.
 * The local storage lasts long enough to fulfill the requirements.
 * The module can display the stored meter values.
 * The module is visible from the out side of the station and allows a comparison with the bill for the user.
 * The displayed values are binding for the contractual relation.
 * The module requires a own a type examination by e.g. PTB

## Requirement fulfillment

The legal requirements:

| Requirement 	| Fulfillment |
|:--------------|:------------|
| Precision 	| ok (external meter) |
| Authenticity 	| ? |
| Integrity 	| ? |
| Imputability 	| ? |
| Availability 	| ok |

The project goals:

| Goal 		| Fulfillment |
|:--------------|:------------|
| User friendly 		| limited |
| Open source 			| no |
| Protocol compatibility 	| ? |
| Roaming-ready 		| ? |


### Legal Requirements

#### 1. Precision

The module connects to a regular metering device which provides the required precision.

> Assumption 1: The connection has to be authentic.


#### 2. Authenticity

The module is built into the charging station and visible from the outside. The user can validate the bill right at the charge point. Therefore the value can be assigned to the exact module, chargepoint and thus the one meter.

> Assumption 2: There will be limitations in the maintenance process when a module or meter gets replaced.

> Assumption 3: The meter values are signed by the module and sent to the MSP for billing.

##### To verify:

 * [ ] Authenticy is fulfilled by the local storage and display alone.
 * [ ] Necessarity of signature validation by the customer
 

#### 3. Integrity

The integrity requirements can be fulfilled by adding a coninuous index into the signed message data.

> See assumption 3.


#### 4. Imputability

> Unknown fulfillment.

##### To verify:

 * [ ] Is this requirement implicitly fulfilled by the design of this solution.


#### 5. Availability

The meter values are saved in the WORM storage in the module of the charge point. Every customer can request to read the stored values and review them on the authentic display of the module.


### Project Goals

#### 1. User friendly

The user has to go back to the charge point to check the meter values on the bill. This can be unconfortable on longer trips and when the bill is sent well after the charging process.


#### 2. Open source

The solution is built into a commercial product. There is no open source specification of the module design known.


#### 3. Compatible with existing protocols

Unclear. Depends on the verification of assomtions.


#### 4. Roaming-ready
 
> Assumption: This solution should be compatible to the current roaming concepts in the market.
