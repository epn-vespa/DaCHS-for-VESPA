# Resource Descriptor file Examples

This directory lists a series of example service configurations. 
They can be used by data providers to train on building their own 
Resource Descriptor files (`q.rd`) and scripts.

## List of available examples

* [BDIP_v2](bdip_v2): Historical images collection in ObsParis, relying on a pre-existing databae. This service illustrates the connection to a remote database in the resource descriptor.
* [CPSTASM](cpstasm): Service for Cluster spectral matrix data in IAP, Prague. Fills the service from local CDF files using cdfHeaderGrammar. 
* [exoplanet](exoplanet): This example retrieves all the data from a distant database.
* [FUB](fub): HRSC/Mars-Express images at Freie Universität, Berlin _(preliminary version, outdated)_
* [Generic service](generic): A generic `q.rd` file based on the Vega/IKS service at Obs. Paris _(caution: this only describes the epn_core table, may be irrelevant when using the `epntap2` mixin)_
* [HISAKI service](hisaki): This test service is based on a sample of the Japanese Hisaki data; it is configured with an external script that fills in the database, and is proposing an `s_region` implementation _(outdated: to be updated with the `epntap2` mixin)_
* [HST_planeto](hst): Retrieves data from a TAP query on a distant service. Defines a datalink parameter to call Miriade ephemeris with current target name and date. 
* [IKS service](iks): Test service for IKS/Vega-1 spectra. Metadata are derived from PDS3 data files and completed with extra information under IDL. Now uses the `epntap2` mixin and csv Grammar.
* [Illu67p](illu67p): This example service has been developed by the CDPP team in Toulouse. It used the new epntap2 mixin feature and a customGrammar to fill the database through DaCHS during the `import` step.
* [IRTF Orton](irtf_orton): This service is using a simple `q.rd` file, and an external Python script to fill the database. This is based on ground based IR observations of Jupiter, in support of Juno. _(outdated: to be updated with the `epntap2` mixin)_
* [Kronos](kronos): This service is a (way too!) complex example of connexion to external database (using PgSQL Foreign Data Wrappers), based on the Cassini/RPWS/HFR database at Obs. Paris, in Meudon. _(outdated: to be updated with the `epntap2` mixin)_
* [MCD](mcd): Service for Mars Climate Database atmospheric simulations in LMD (profiles only). 
* [myPoly](mypolyb): This a test service that implements `s_region` with the `sPoly` type from PgSphere.
* [ObsNancay NDA-old](nancay_dam): This is an old version of the Nancay Decameter Array service. _(outdated: to be updated with the `epntap2` mixin)_
* [ObsNancay NDA-new](nda-epntap2-mixin-customGrammar): This the new version of the previous example. This example proposes a complete tutorial for setting up similar services (using daily CDF files). It contains the `epntap2` mixin and uses a customGrammar.
* [Planets](planets): A small generic service, with the main parameters of Solar System planets. Illustrates a service built from a csv file. Now uses the `epntap2` mixin and csv Grammar.
* [PlanetServer-CRISM](planetserver_crism): Service providing hyperlinks and access URLs to PlanetServer2 interface and CRISM-derived data products.
* [PlanetServer-M3](planetserver_m3): Service providing hyperlinks and access URLs to PlanetServer2 interface and M3-derived data products.
* [PDS_speclib](PDS_speclib): For PDS spectral library service. Uses the `epntap2` mixin and csv Grammar.
* [SBNAF](sbnaf): IR flux of asteroids measured through several observatories, outcome of SBNAF EC programme in Konkoly Obs (alternative access through EPN-TAP). All data are in the table, no attached files. Defines a datalink parameter to call Miriade ephemerides with current target name and date. 
* [spectro_planets](spectro_planets): For Telescopic Planetary Spectra collection. Uses the `epntap2` mixin and csv Grammar.
* [spicam](spicam): Service for SPICAM/Mars-Express atmospheric profiles in LATMOS. Defines a datalink parameter to 1) call the Mars Climate Database (with free parameter selecting the scenario in use) 2) provide a link to an alternative (ascii) version of the file
* [VVEx](vvex): An example service for VIRTIS-VEx data using IDL to build the ingestion SQL script.  _(outdated: to be updated with the `epntap2` mixin)_


## More info

More tutorials and informations on how to set up a service are available from:

* the [VESPA discussion and documentation wiki](https://voparis-confluence.obspm.fr/display/VES/Implementing+a+VESPA+service)
* the [GAVO/DaCHS documentation web site](http://docs.g-vo.org/DaCHS/)


