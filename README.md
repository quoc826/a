"MATCH (s:Supplier {company_name: $name})-[r]-(p:Product) " +
"RETURN p";


"MATCH (s:Supplier {supplier_id: $id}) "+
"SET s.company_name = $name " +
"RETURN s";
