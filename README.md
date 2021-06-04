# Ayesha-Beauty-Creation-Database
https://datatofish.com/how-to-connect-python-to-ms-access-database-using-pyodbc/ (link to how to use the database)



import pyodbc

conn = pyodbc.connect(r'Driver={Microsoft Access Driver (*.mdb, *.accdb)};DBQ=C:\Users\Ananias Amanyanga\Desktop\Python\Ayesha Beauty Creation Database.accdb;')
cursor = conn.cursor()
cursor.execute('select * from Customer')
   
for row in cursor.fetchall():
    print (row)
