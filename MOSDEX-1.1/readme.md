

Provides a JSON Schema specification for MOSDEX version 1.1 and example MOSDEX files validated under that schema.

Synopsis of Changes In v1-1 vs. v1-0
<ul>
<li>Implemented the MOSDEX syntax as a JSON Schema</li>
<li>Added a Syntax field to the MOSDEX file to verify the version of the JSON Schema used</li>
<li>Exposed the Table class as a general artifact that can be used in future extensions of MOSDEX</li>
<li>Replaced the Role field of Table and its subclasses with a mandatory Type field, whose allowable values depend on the class, and put the role information in it; added a Type field to the subclass schemas</li>
<li>Added an Expression subclass of Table for specifying nonlinear problems using expression graphs</li>
<li>Renamed the Expression field in Heading as Math to avoid name conflict with the Expression class</li>
<li>Renamed the Coefficient subclass of Table as Term and created separate schemas for linear, quadratic and nonlinear types to accommodate the corresponding number and types of arguments</li>
</ul>

