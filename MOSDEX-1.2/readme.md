

Provides a JSON Schema specification for MOSDEX version 1.2 and example MOSDEX files validated under that schema.

Synopsis of Changes In v1-2 vs. v1-1
<ul>
   <li> Revised the Recipe object as an array of Clause objects, each of which specifies an SQL directive and its predicate. Fuller explanation of how SQL Recipes work.</li> 
   <li> Added an optional Keys field to Table and its subclasses for use in queries with string substitution.</li>
   <li> All fields of Heading are arrays of strings, for consistency.</li>
   <li> Use #Solver prefix on calls to solver methods.</li>
</ul>
