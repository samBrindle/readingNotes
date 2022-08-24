# Readings: Django Models
## Using Models
Django uses Python objects referred to as models to access and manage data.
* These models define the structure of stored data
  * field types
  * maximum size
  * default values
  * selection list options
  * many other things
### Designing the LocalLibrary models
* Always think about what data you are storing and the relationships between different objects
  * Ex: Storing info about books:
    * Title, Summary, Author, ISBN, ect
* Use separate models for every "object" (group of related info)
  * Ex: Books and Authors

### Model Primer

#### Model Definition
* Models are defined in models.py
* Implemented as subclasses of `django.db.models.Model`

#### Fields
* A model can have any number of field of any type
* Each one represents a column of data
* The field name is used to refer to it in queries and templates

#### Common Field Types
* CharField - short to mid sized fixed length strings
* TextField - large, arbitrary length strings
* IntegerField - Storing integer values
* DateField and DateTimeField - use for storing dates and date/time info
* EmailField - stores and validates email addresses
* FileField and ImageField - used to upload files and images
* AutoField - special type of IntegerField that automatically increments
* ForiegnKey - used to specify a one-to-many relationship in another DB
* ManyToManyField - used to specify a many-to-many relationship

#### Metadata
* Useful to control the default ordering of records returned from a query

## Django Admin Site
### Registering Models
* Open admin.py and add in `admin.site.register(*Model*)`

### Creating a superuser
* `python3 manage.py createsuperuser`
  * will ask you for a username, email, and password
* After logging in on the admin site with a superuser you can create users, groups, and add to DB's 
