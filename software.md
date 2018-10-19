### Software/tools 
1. [iRODS](https://irods.org/) 
2. [Denodo](https://www.denodo.com/en) 
3. [CKAN](https://ckan.org/) 
4. [Figshare](https://figshare.com/) 
5. [Immuta](https://www.immuta.com/) 
6. [Metadata Management for Applied Sciences (MASi)](https://www.sciencedirect.com/science/article/pii/S0167739X17305344) 
7. [Starfish](http://www.starfishstorage.com/) 
8. [StrongLink](https://www.strongboxdata.com/stronglink) 
9. [Clowder](https://clowder.ncsa.illinois.edu/) 
10. [GIN](https://web.gin.g-node.org/) Modern Research Data Management for Neuroscience
11. [Datalad](https://www.datalad.org/) 
12. [Claritynow](https://dataframeworks.com/products/claritynow)
13. HPE [DMF](https://www.hpe.com/us/en/product-catalog/detail/pip.hpe-data-management-framework.1010144088.html) 
14. [Pentaho](https://www.hitachivantara.com/go/pentaho.html) 
15. [Cloudian](https://cloudian.com/solutions/data-management/) 
16. [Arvados](https://arvados.org/) 
17. [Datera](https://datera.io/) 

### Categories 

The software/tools in this list can be categorized the following way based on functions and requirement it fulfils.

(Data Management Abstraction and Layers)

* Storage Abstration Layer 
* Data Virtualisation / Data Source Discovery Layer 
* Data Movement Layer 
* Fedreation Layer 
* Consuming/Publishing Layer 
* Policy 
* Metadata 

### Details 


1. [iRODS](https://irods.org/) 

<b> Description/Common usage</b>

Used for data virtualization, federation, discovery (from variety of storage resources), workflow automation via policy engine. This is a <b> open source </b> project maintained by the iRODS consoritum. 
  
 The architecture code base is n c++. There is a SQL database backend for the catalog. Various API options are available.  
 iRODS provide a flexible rule engine language that can enforce policy on various data collections and objects. 

Native authentication, PAM (e.g. redirecting to LDAP) / SSL , GSI, Kerberos


“The iCAT server stores metadata in the form of “triples” to its relational database. The triples consist of an attribute field, a value field, and a unit field. The content of each of these fields can be independently defined and applied. Metadata may be user-defined or applied automatically. By default, iRODS does not automatically apply any user-accessible metadata; the zone administrator must implement metadata automation in the iRODS rule engine.” (irods.org)


Various plugin interfaces that are configurable can access various storage backends. 
- Data access is given by the iRODS native protocol and a commandline tool. (SSL)
- Webdav: stable community software to extend iRODS with the webdav protocol which allows for data mounting and web access to data. Supports also editing data directly in iRODS with office programs (SSL)
- gridFTP: Supported by EUDAT, stable extension to iRODS to allow data access by gridFTP for large data transfers (encryption)

IRODS have various features for this. Dynamic policy enforcement, rule engine.  iRODs also have federation feature where various geographically distributed 

Rule engine (processing of small datasets and metadata can be added/customizable). 
With QueryArrow one can query different iCAT catalogues no matter on which database technology they are built. With rule engine iRODS can work with datasets (i.e. subsetting of queried data, merging of different datasets and reformatting of data and metadata). Rule engine can also invoke external processing tools. 

GUI/publishing layers: 

Metalnx/YODA/iRODS ticket system/iRODS anonymous user+webdav/bridge to various other repositories. 

2. [Denodo](https://www.denodo.com/en) 

Creates a data virtualization layer by connecting various  structured data sources. Provides  unified access for consuming applications. Not open source but a free express version is available. There is an active user community (contains open forum/mailing list). 

One the main advantages of Denodo is that the datasets (or databases) do not need to be physically copied or moved. For example, if we need to combine a mySQL database and a csv file, usually one have to import the csv file into the database first and then run the queries. In Denodo part of the data cane be copied to the cache instead of the whole datasets. The Denodo server pushes down as much processing as it can to the data sources, but it still has to retrieve the data from them and perform the join. 

There is also a nice RESTful API option that can provide access to customized reports/views. 


3. [CKAN](https://ckan.org/) 

Data portal, repository. Open Source. 

4. [Figshare](https://figshare.com/) 

Digital repository / data publishing platform. Commercial/ not open source. 


5. [Immuta](https://www.immuta.com/) 

Focused on big data and data science applications (provides data management and portal solution). 


6. [Metadata Management for Applied Sciences (MASi)](https://www.sciencedirect.com/science/article/pii/S0167739X17305344) 

At present this seems to be more of a research project that a deployable solution. Open Source?? 


7. [Starfish](http://www.starfishstorage.com/) 

"Whether 1 million files and TBs of data or 10s of billions of files and petabytes of data, Starfish scales with you. Track trends, drill down to file level, search and query, run jobs, kick off workflows, and simultaneously scan and move files between any posix-like filesystem. Commercial grade code allows you to install Starfish in 15 minutes and benefit from non-disruptive upgrades."

Commercial/ not open source 
Possible fit in both structured and non-structured data. 


8. [StrongLink](https://www.strongboxdata.com/stronglink) 

Provides a gloabl namespace, automated data migration and also policy based data lifecyle management. 

 Commercial. 

9. [Clowder](https://clowder.ncsa.illinois.edu/) 

Open Source. 
Nice API. lots of focus on Metadata integration, extraction. 


10. [GIN](https://web.gin.g-node.org/) Modern Research Data Management for Neuroscience

Using GIT annex for data management and version control. 


11. [Datalad](https://www.datalad.org/) 

Another project using GIT annex. Also can search external data repository. 

This can be a nice solution to combine a large data set (either ingested via webDAV or connecting to a exsiting resource) with code repository and have a git like view to management and see the data structures. 


12. [Claritynow](https://dataframeworks.com/products/claritynow)


13. HPE [DMF](https://www.hpe.com/us/en/product-catalog/detail/pip.hpe-data-management-framework.1010144088.html) 

14. [Pentaho](https://www.hitachivantara.com/go/pentaho.html) 
Commercial. 
BI tool. 

15. [Cloudian](https://cloudian.com/solutions/data-management/) 
Commercial 

More of a storage management solution. However can be customized to create policies to managed tiered storage and hybrid clouds. 

16. [Arvados](https://arvados.org/)

Open source (focused on bioinformatics) 
With CWL (Commmon workflow language). 


17. [Datera](https://datera.io/) 
Commercial. 
