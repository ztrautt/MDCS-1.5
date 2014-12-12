Materials Data Curation System
==============================

The Materials Data Curation System (MDCS) allows for the curation of materials data into a repository using predefined templates. The system also allows for browsing and exploring of the materials data using the predefined templates as well.

The software was developed by the National Institute of Standards and Technology (NIST)

<h3>Disclaimer</h3>

The XML-based schemas provided with the Materials Data Curator are examples of schemas that may be written to represent different aspects of materials data and to demonstrate some of the features that may be used within an XML schema (i.e. including tabular data or composition selection using the periodic table). The schemas do not represent “standard” metadata representations and are specifically release as “as is,” and as such NIST makes no warrant of any kind on the correctness or accuracy of the content of the schemas, nor the fitness of the schemas for any purpose and accepts any liability or responsibility for the consequences of the schemas use or misuse by anyone. 

Note the Demo-Diffusion_v2 data schema is not meant as a metadata standard for diffusion data.  It is just an example of how one might specify some of the metadata associated with typical tracer, intrinsic and chemical (interdiffusion) diffusivity experiments. This schema can be customized to fit the users’ needs. It should also be noted that while the Demo-Diffusion_v2 schema contains some instruments types  (e.g Electron Probe Micro Analyzer or a microtome) not all the appropriate metadata for each instrument has been defined nor have all of the appropriate instrument types been defined. 

Also note that not all XML-schemas will load properly within the Materials Data Curator.

<h3>Notes</h3>
<h4>Modules</h4>
The MDCS allows integration of modules to provide better user interfaces for entering data. The integration of modules is done by giving a tag name from the XML schema. The tag is then replaced by the module when the form to enter data is rendered. For convenience, some modules are present by default for materials scientists working on the demo-diffusion.xsd template (provided with the sources). The XML tags with the following names will be automatically replaced by the corresponding module:
-	ConstituentsType
-	ChemicalElement
-	Table

<h4>Import</h4>
The MDCS allows to upload schemas that may contain import statements. Schemas that can be imported in other schemas should be uploaded first in the system. Then, when uploading a schema containing import statements, the value of the schemaLocation attribute of the import statement should match the name of one of the previously uploaded schemas. The schemaLocation attribute should only provide the file name. Neither absolute or relative path would be interpreted as such. 
