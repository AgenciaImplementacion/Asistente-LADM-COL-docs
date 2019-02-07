Settings
************

.. image:: static/03_CONFIGURACION.gif
   :height: 500
   :width: 800
   :alt: basic settings

Database Connection
---------------------

In this tab, the parameters are defined to connect to the database in which the
physical model of LADM_COL is stored.

These parameters are: \

*Common parameters*

**Source**: define the origin of the data, it can be a spatial database
*PostgreSQL/PostGIS* or *GeoPackage*.

*Only PostgreSQL/PostGIS parameters*

**User**: User name that has permission on the database

**Password**: user password

**Host**: address where the database is hosted *localhost* is equivalent to
*127.0.0.1*

**Port**: listening port number for the database

**Database**: Name of the database that contains or will contain the physical
model of LADM_COL

**Schema**: Name of the schema that stores the objects of the physical model of
LADM_COL

.. image:: static/db_connection_settings.gif
   :height: 500
   :width: 800
   :alt: set database connection settings

**Note**: You can create your database and schema. But names should not contain special characters.

*Only GeoPackage parameters*

**Database File**: Disk location of the GeoPakage file that contains the
database.

The *Test Connection* button is used to know if the entered parameters are
correct and allow connection to the database

Models
-------------
In this tab, you can select whether you want to use the repository of local or remote models.

.. image:: static/set_custom_models_directories.gif
   :height: 500
   :width: 800
   :alt: set custom models directories

Quality
-------------

For data quality issues in this tab, the tolerance limit allowed for
too long boundary segments is established, this must be defined in meters.

Automatic Values
-----------------

Most of the classes in LADM_COL have two attibutes that combined must be unique
in the whole ``schema/database``. They are called **namespace**
and **local_id**. To make it easier to fill those attibutes, the *LADM_COL
assistant* can set automatic values for them.

Namely, **namespace** will correspond to an optional pefix (e.g.,
MY_ORGANIZATION) plus the class name (e.g., BOUNDARY):
`MY_ORGANIZATION_BOUNDARY`.

On the other hand, **local_id** will correspond to the id of the record in the
database.

If you want to fill those values by youtself, uncheck the check boxes in this
form.

.. image:: static/settings.gif
   :height: 500
   :width: 800
   :alt: about plugin


Sources
-------

It's possible to configure through a data repository a URL path to upload
administrative sources and spatial sources associated with the information
collected in LADM-COL.

.. image:: static/Configurar_fuentes.gif
   :height: 500
   :width: 800
   :alt: Setting up sources
