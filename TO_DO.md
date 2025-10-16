# 📋 Project To-Do List

## 👤 Person 1 – Data Modeling & Integration

**Goal:** Design the semantic backbone and populate the graph.

### Main Tasks

- [ ] **Define Vocabulary (RDFS)**
  - [ ] Create `cto_schema.ttl` with core classes and properties.  
  - [ ] Reuse and align with **FOAF**, **GeoSPARQL**, and **Schema.org**.

- [ ] **Design Validation Shapes (SHACL)**
  - [ ] Write `cto_shapes.ttl` with structural and datatype constraints.  
  - [ ] Add SPARQL-based rules for temporal and cross-entity checks.

- [ ] **Build RDF Data Graph**
  - [ ] Produce `cto_data.ttl` (or multiple files) with rich instances.  
  - [ ] Link to **DBpedia** or **Wikidata** for cities, regions.

- [ ] **Validate and Iterate**
  - [ ] Run **SHACL validation** and fix inconsistencies.  
  - [ ] Deliver **diagrams** of class and property structures for the report.
  

## 👤 Person 2 – SPARQL Queries & Documentation

**Goal:** Implement query logic, testing, and final packaging.

### Main Tasks

- [ ] **Develop Competency Questions**
  - [ ] Write **15 user-oriented queries** in `cto_query.txt`.  
  - [ ] Cover:
    - Selection  
    - Aggregation  
    - Path expressions  
    - `FILTER`s, `OPTIONAL`s, `UNION`s, and subqueries

- [ ] **Build Testing and Automation Scripts**
  - [ ] Validate RDF syntax and SHACL shapes.  
  - [ ] Run queries against the dataset for verification.

- [ ] **Write Report (≤ 5 pages)**
  - [ ] Summarize:
    - Schema design  
    - Modeling rationale  
    - Query coverage  
  - [ ] Include an **AI-tool disclosure section**.

- [ ] **Package Project**
  - [ ] Prepare final **ZIP** with all files, directory structure, and `README.md`.  
  - [ ] Ensure **reproducibility** and internal cross-references.

---

## ✅ Deliverables Summary

- [ ] `cto_schema.ttl` – ontology definition  
- [ ] `cto_shapes.ttl` – SHACL validation shapes  
- [ ] `cto_data.ttl` – RDF data instances  
- [ ] `cto_query.txt` – SPARQL competency queries  
- [ ] `report.pdf` – project summary  
- [ ] `README.md` – documentation and usage guide
