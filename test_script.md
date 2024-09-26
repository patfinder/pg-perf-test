
# ============= Insert/Update rows

# Create table with some missing/deleted rows

# Create temp table with all rows

# Run upsert: insert on conflict update



# Write python script to delete some rows

```sql

INSERT INTO products
SELECT * FROM temp_products t
WHERE t.id = 56414
ON CONFLICT (id) DO UPDATE
SET name = EXCLUDED.name;

ALTER TABLE products
ADD PRIMARY KEY (id);


select t.id, p.name, t.name from products p right outer join temp_products t on p.id = t.id where t.id = 56414 limit 3;


gen_data 500k.csv -r500000 -d -c"2,3:100,3:8,3:100,4,2" -t"id,name,sku,description,price,stock" 

-- 56414 66609 10627 56196 77345 20943 73023 85392 94248 68518

```

```python

# delete some random row
def do_upsert():
    # Read csv file.

    # Loop 

```

