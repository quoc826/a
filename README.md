CREATE INDEX index_supplier IF NOT EXISTS
FOR (s:Supplier)
ON (s.supplier_name)


CREATE CONSTRAINT unique_supplier IF NOT EXISTS
FOR (s:Supplier)
REQUIRE (s.supplier_id) IS UNIQUE
