# darwincore_omeka
A guide on how to use [Darwincore RDF](https://dwc.tdwg.org/rdf/) with [Omeka S](https://omeka.org/s/). 

## Adding the Darwin Core RDF terms to Omeka 
In Omeka, follow these steps:
1. Go to Vocabularies in the sidebar
2. Import new vocabulary in the top-right hand corner
3. Add the following in their respective fields  
    * **Label**: `DarwinCore`  
    * **Namespace URI**: `http://rs.tdwg.org/dwc/terms/`
    * **Prefix**: `dwc`
    * **Vocabulary URL**: `http://rs.tdwg.org/dump/terms.ttl`
4. Click `Import`
5. Enjoy the new vocabulary!

It'll be useful to have some resource templates. Go ahead and add them using the following steps.

## Adding Darwin Core resource templates for classes
1. Download the relevant resource template file from this repository (e.g. `Taxon.json`)
2. Click `Import` in the top-right hand corner
3. Select the file downloaded in step 1 and click `Review import`
    * You will see a table listing all fields, with the data types, alternate tables, etc...
4. Click `Complete import`
5. Try it out! Create a new item using the template.

> [!TIP]
> You can edit the resource template to give any of the fields an alternate label, description, default language, data type, mark a field as resource title, description, required, and private.
> 1. Go to resource templates
> 2. Click on the template that you want to edit
> 3. Click on `Edit resource template`
> 4. On the field that you want to edit, click on the pencil icon, and make your edits
> 5. Don't forget to save!


### Available resource templates 
The following classes are available as resource templates in the `resource_templates` folder. I'll keep adding to those in the coming days, but also please feel free to make a PR with the relevant resource templates, and I'll be happy to merge those. 
* `Generic_Darwin_Core_Record`: Record-level properties that are generic in that they might apply to any type of record in a dataset. 
* `Taxon`
