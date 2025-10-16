# Cycling Tour Operator – Linked Data Mini Project

This workspace models a cycling tour operator as RDF, validates it with SHACL, documents the custom vocabulary with RDFS, and provides example SPARQL queries.

Files
- cto_data_xxx.ttl: Instance data (destinations, paths, bikes, tours, bookings, people, cities, countries). Linked to DBpedia via owl:sameAs for selected resources.
- cto_shapes.ttl: SHACL NodeShapes to validate the dataset (e.g., TourPackage, Booking, BikeModel, RentalBike, City, Country).
- cto_schema.ttl: RDFS schema for the custom cm: vocabulary, reusing FOAF and W3C ORG where appropriate.
- cto_query.txt: 15 SPARQL queries demonstrating common questions over the graph.

Validate with SHACL
The shapes and data conform. To re-run validation locally:
- Ensure a Python environment with pySHACL and rdflib is available.
- Example command (adjust path to your interpreter if needed):
	python -m pyshacl -s cto_shapes.ttl -d cto_data_xxx.ttl -f human

Run the SPARQL queries
You can execute the queries in cto_query.txt with any SPARQL engine that can load local Turtle files (e.g., RDF4J Workbench, Apache Jena ARQ). Load cto_data_xxx.ttl and run the selected query blocks.

Notes
- GeoSPARQL geometries were intentionally omitted.
- Bike modeling distinguishes catalog models (cm:BikeModel) from physical instances (cm:RentalBike).
- Organization uses W3C ORG for membership and offering relations (cm:offersTourPackage, cm:offersBikes).
- SHACL shapes and data are kept in sync; status and enumerations use properly typed xsd:string literals.