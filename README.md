[![Travis](http://img.shields.io/travis/csgf/scoap3-harvester-api/master.png)](https://travis-ci.org/csgf/scoap3-harvester-api)
[![Documentation Status](https://readthedocs.org/projects/csgf/badge/?version=latest)](http://csgf.readthedocs.org)
[![License](https://img.shields.io/github/license/csgf/scoap3-harvester-api.svg?style?flat)](http://www.apache.org/licenses/LICENSE-2.0.txt)


#scoap3-harvester-api


The project aims to do harvesting of the SCOAP3 resources ,using API KEY, and insert them into Open Access Repository(http://www.openaccessrepository.it)


There are 3 classes:
- Scoap3withAPI.java is the main class. 
 	It’s mandatory to put  your private and public key to do a query.(String privateKey and      String 	publicKey)
	Using the startDate parameter, you can find all records created from start date(String startDate)

-Scoap3_step2. java is a class to separate the INFN resources from OTHERS.

-HmacSha1Signature. java is a class to generate the signature from private key.

The script returns a folder that contains :
-INFN folder (all INFN resources in MARCXML format )
-OTHER folder ((all OTHER resources in MARCXML format )
