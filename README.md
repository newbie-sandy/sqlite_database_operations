# Details on the datasets you've selected
- Pricing transparency dataset of Stonybrook Hospital
# An account of the exploratory data analysis process
## Date cleaning
- identify duplications, null values
## Univariate analysis and visualization
- using Plotly to visualize the distribution of 'Gross charge'
## Instructions to replicate your SQLite database setup
### Create db. 
import sqlite3
connection = sqlite3.connect("health.db")
cursor = connection.cursor()

### Creat table
connection.execute("""
 CREAT TABLE name
        (column_1 DTYPE PRIMARY KEY,
        column_2 DTYPE,
        ... DTYPE,
        column_n DTYPE)
  """)

### Insert rows manually
health = ("""
INSERT INTO name
(column_1,
column_2,
...,
column_n)
VALUE(
     value_1,
     value_2,
     value_n
  )
""")
connection.commit()
connection.close()

# Any other pertinent documentation or guidelines
 - Unsolved problems
   Haven't figured out the to_sql function yet. I created the new sqlite database and the table but failed to push the csv. to it.
