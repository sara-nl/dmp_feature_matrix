Software/tools: 

1. [iRODS](https://irods.org/) 
 

<b> Description/Common usage

Used for data virtualization, federation, discovery (from variety of storage resources), workflow automation via policy engine.


<b> Open Source 
  
  Yes. 
  
<b> Architecture/Infrastructure</b>
  
* code base in c++
* SQL database backend 
* API/FUSE 
* Flexible rule engine 
* Native authentication, PAM (e.g. redirecting to LDAP) / SSL , GSI, Kerberos
  
<b> Metadata management and extension</b>

“The iCAT server stores metadata in the form of “triples” to its relational database. The triples consist of an attribute field, a value field, and a unit field. The content of each of these fields can be independently defined and applied. Metadata may be user-defined or applied automatically. By default, iRODS does not automatically apply any user-accessible metadata; the zone administrator must implement metadata automation in the iRODS rule engine.” (irods.org)

<b> Policy Enforcement</b>


<b>Layers: </b>

We identified three layers: a) Data Source Layers b) Data Integration Layer c) Data Publisher Layer 

DSL:
  
Various plugin interfaces that are configurable can access various storage backends. 
- Data access is given by the iRODS native protocol and a commandline tool. (SSL)
- Webdav: stable community software to extend iRODS with the webdav protocol which allows for data mounting and web access to data. Supports also editing data directly in iRODS with office programs (SSL)
- gridFTP: Supported by EUDAT, stable extension to iRODS to allow data access by gridFTP for large data transfers (encryption)

Data Integration Layer: 

IRODS have various features for this. Dynamic policy enforcement, rule engine.  iRODs also have federation feature where various geographically distributed 

Data Publishing Layer: 

Metalnx/YODA/iRODS ticket system/iRODS anonymous user+webdav/bridge to various other repositories. 

<b>Sharing/Publications: </b>

<b>Processing/Analysing tools </b>
Rule engine (processing of small datasets and metadata can be added/customizable). 
With QueryArrow one can query different iCAT catalogues no matter on which database technology they are built. With rule engine iRODS can work with datasets (i.e. subsetting of queried data, merging of different datasets and reformatting of data and metadata). Rule engine can also invoke external processing tools. 


<b> Graphical Interface: </b>
YODA 


2. [Denodo](https://www.denodo.com/en) 
Creates data virtualization layer by connecting various  structured data sources. Provides  unified access for consuming applications.

3. [CKAN](https://ckan.org/) 
Data portal, repository

4. [Figshare](https://figshare.com/) 
Digital repository 

5. [Immuta](https://www.immuta.com/) 
Focused on big data and data science applications (provides data management and portal solution) 

6. [Metadata Management for Applied Sciences (MASi)](https://www.sciencedirect.com/science/article/pii/S0167739X17305344) 

7. [Starfish](http://www.starfishstorage.com/) 

8. [StrongLink](https://www.strongboxdata.com/stronglink) 

9. [Clowder](https://clowder.ncsa.illinois.edu/) 

10. [GIN](https://web.gin.g-node.org/) Modern Research Data Management for Neuroscience

11. [Datalad](https://www.datalad.org/) Datalad
