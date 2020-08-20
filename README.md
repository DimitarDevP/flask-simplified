# flask-simplified

 A reworked version of the FlaskSQL extension by DimitarDevP
 
# Main Differences

 - Dropped flask_mysqldb support as it is slow and uncapable of connecting to databases other then MySQL.
 - Replaced flask_mysqldb with SQLAlchemy.
 - Separated the codebase into 2 different classes - one for app initialization and one for working with database.
 - Added a query prepare method which generates a MySQL query from a python dictionary.

# MAJOR NOTE TO SELF:

 - I will move the entire FlaskSQL module to C++ and compile it to a Python module for better performance
 - I will abstract the code further to make the creation of basic CRUD operations for interacting with tables much easier.
