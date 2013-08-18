Los Angeles Community Resources
======================

Postgres database containing social programs in and around Los Angeles, CA. Data current as of August 2013. The database has a number of tables, but those relevent for extracting community resource data are:

* agency: Information about the organization (i.e. United Way)
* program: Information about a program provided by an agency (i.e. children's after school program)
* site: A location for a program (i.e. one of an arbitrary number of physical locations for the children's after school program)

Each of the tables above have corresponding <code>*_text</code> fields to handle localization.

In a few places you will see the prefix <code>sn_*</code> for table names. The <code>sn</code> was an internal code-name for Safetynet, the original name of the Idealistics Community Resources product.

As stated earlier, there are some other pieces to the database that aren't terribly relevent to those looking to pull this resource data into alternative resource databases. That said, you are free to use this database in its entirety as you please.

Setup
-----------
The setup script, <code>la_community_resources.sql</code> was built under Postgres 8.3. The script uses insert commands, so give it a moment or two to run.

To load the database, simply create a databse with whatever name of your choosing and execute the script.

History
-----------
From 2007 - 2013, Southern California based Idealistics Inc. worked with non-profit and goverment social sector organizations to populate and mantain a database that matched low-income individuals and families to social programs. Idealistics decided to close in the summer of 2013 and opend up this databse to the community.

License
---------------
MIT. Do good in the world.
