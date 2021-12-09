New MOSDEX syntax summary:
<ol>
  <li>Eliminated named objects (Problems and Tables)</li>
  <ol>
<li>All objects now have a keyword as field name</li>
<li>The MOSDEX File has a Modules array</li>
<li>The MOSDEX Module has a Tables array</li>
<li>Problem has been renamed Module</li>
  </ol>
<li>New syntax for schema</li>
    <ol>
<li>Eliminated named fields in favor of two arrays: FIELDS and TYPES</li>
<li>Horizontal layout aligns over the instance columns and eliminates a separate Fields array (this is not part of the standard; JSON doesn’t care about the layout)</li>
        </ol>
<li>Function calls</li>
    <ol>
<li>Needed for retrieving the solution</li>
<li>Define a data type for function calls for use in the schema</li>
<li>Parse the function call from a string in the MOSDEX File</li>
    </ol>
<li>Type (schema) information added in SELECT Queries</li>
    <ol>
<li>MOSDEX supports data types (IEEEDOUBLE, Function calls) that are not supported in SQL.</li>
<li>MOSDEX needs to carry this type information through its data transformations from input -> model -> output</li>
<li>Solution: add the type information as comments (denoted by --) in the SQL</li> 
    </ol>
<li>Solver result calls are specified as part of the relevant modeling object</li>
    <ol>
<li>Results can be reformatted as OUTPUT DATA tables using SQL.</li>
    </ol>
<li>UPDATE query field added to table to facilitate iterative modular structures</li>
    <ol>
<li>e.g. decomposition</li>
    </ol>
  </ol>
