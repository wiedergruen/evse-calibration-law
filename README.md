## Motivation

The goal of this open source project is to handle the German calibration regulation requirements for charging stations and associated parties. The problematic is the compliant billing of charging electric vehicles with public charging stations. 

For compatibility and standardized interfaces of different parties, its open source. The goal is to develop a harmonized solution that can be implemented by all parties in the market, providing one simple solution for all customers.

#### Background

The German calibration law regulates the calibration and processing of measurement instruments and the non falsifiability of its measured values. Therefore its required that consumers/users can check the originality of measured values, to be sure the billing is correct. 


## Table of Contents

 * [Scope](#Scope)
 * [Supporters](#Supporters)
 * [Links](#Links)
 * [FAQ](#FAQ)
 * [Contribution](#Contribution)
 * [License](#License)


## Scope



### Transparency Software

This software confirms the measured values signature with the charging stations public key (smart meter gateway public key). It can be available as a mobile app or as a webapp. So everyone can check the measured values signatures.


### Interfaces

Required interfaces for conform billing.

#### Online interfaces

 * EVSE - CPO Backend: Sending of signed meter values
 * CPO Backend - MO Backend: Forward the signed values for billing
 * CPO Backend - roaming platform: Forward signed values to the right roaming partner
 * MO Backend - transparency software (user): Bill and the signed values

#### Offline interfaces

 * EVSE - transparency software (user): Manual public key saving

#### Public Key

The public key is available for the user offline, imprinted at the charging station. The public key is necessary to confirm the gateways signature. 

## Supporters

 * [Wiedergrün](https://wiedergruen.com)
 * [SMATRICS](https://smatrics.com)

## Links

 * [MessEG](https://www.gesetze-im-internet.de/messeg/BJNR272300013.html)
 * [MessEV](https://www.gesetze-im-internet.de/messev/BJNR201100014.html)
 * [BNetzA Ladesäulenkarte](https://www.bundesnetzagentur.de/DE/Sachgebiete/ElektrizitaetundGas/Unternehmen_Institutionen/HandelundVertrieb/Ladesaeulenkarte/Ladesaeulenkarte_node.html)


## Contribution

Any productive contributions are welcome!

 * Post thoughts about new features as issues
 * Post questions as issues or get in touch directly
 * To correct bugs send us pull request

If you are interested to work more intensive in this project, send us your request via our company homepages contact form at [wiedergruen.com](https://wiedergruen.com/).

## License

MIT see file [LICENSE](LICENSE).




