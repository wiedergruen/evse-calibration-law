# Key Requirements

The following key requirements have to be solved for a law conform metering system.

### 1. Precision

The value of the measured variable must get assigned as accurately as possible by a metering device to the true value according to the physical conventions.

### 2. Authenticity

After transmission of a message, the metering value must be assignable to a specific data source.

### 3. Integrity

It must not be possible to falsify the content of a transmitted message without recognition. It must not be possible to append additional apparent messages and no messages must get lost undetected.

### 4. Imputability

A measured value in a transmitted message must be undoubtedly and confidently assignable to the person which is liable for the bill in association with the measurement.

### 5. Availability

A measured value must be available to the contractors of a transaction until the process, including the agreed payment of the invoice, is completed.



# Requirements mapping

Those requirements can get mapped to the system parts and be extended to describe the practical minimal system requirements to be implemented.

### Metering Instrument

 * meter values are safe against falsification
 * meter accuracy class A
 * right operation enviroment, (e.g. temperature of operation)
 * PTB type approval exists ("PTB Bauartzulassung")
 * certificated meter software
 * interface cannot change essential system parameters
 * possible certificated software updates
 * every change must be noted undeletable

### Additional Meter Units

 * meter value signing
 * imprinted public key and the user can clearly read it
 * safe against falsification
 * certificated software
 * possible certificated software updates
 * every cahnge must be noted undeletable
 * user interface to see saved meter values
 * ergonomic user interface
 * user interface cannot change essential system parameters
 * TCP as chosen protocol
 * the private key cannot be compromised without breaking a seal

### Transperancy Software

 * GUI for users
 * can check the meter hash
 * manual public key input
 * web interface to get public keys via a public database

### Interfaces

 * TCP as chosen protocol
 * no data falsification possible
 * interoperability

### Overall System

 * no falsification of meter values possible
 * user gets signed meter values on his invoice
 * critical mutual influence of systems are not possible
 * charge points own energy consumption is not billed to the customer
 * the customer is just billed for his amount of charge




 
