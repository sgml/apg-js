##JavaScript APG

**Version:**  1.0

**Description:**  
<ul><li><b>JavaScript APG</b> is a version of <a href="http://www.coasttocoastresearch.com/">APG  &ndash; an ABNF Parser Generator</a> written entirely in JavaScript.</li>
<li>generates recursive-descent parsers directly from ABNF (<a href="https://tools.ietf.org/html/rfc5234">RFC5234</a>) grammar specifications</li>
<li>no target-language code imbedded in the grammars</li>
<li><code>AND</code> and <code>NOT</code> syntactic-predicate operators for conditional parsing based on look-ahead phrases</li>
<li>user-written callback functions allow recognition of non-Context-Free language phrases</li>
<li>user-written callback functions provide complete monitoring and flow control of the parser</li>
<li>optional generation of an Abstract Syntax Tree (AST)</li>
<li>translation of the AST with user-written callback functions</li>
<li>extensive tracing facilities</li>
<li>statistics gathering for a full picture of parse tree node coverage</li>
<li>extensive attribute generation for an overview of the grammar's characteristics</li>
</ul>

<i>NOTE: Currently this repository includes only the APG runtime library required for running APG-generated parsers.
The generator itself is currently only available at the <a href="http://www.coasttocoastresearch.com/interactiveapg/">APG website</a>.
Full instructions for building a parser are given in the example files.</i>

**Files:**  

|file name|description|
|:--------|:----------|  
|  apgAst.js                   |the AST class, required for generating an AST from the parse|
|  apgLib.js                   |the APG runtime library, required for all JavaScript parsers|
|  apgStats.js                 |the Stats class, required for collecting parsing statistics|
|  apgTrace.js                 |the Trace class, required for tracing the parser&acute;s path through the parse tree|
|  apgUtilities.js             |a collection of optional, but useful utilities, many to assist output of results|
|  example/example.css         |a simple stylesheet for the example HTML page|
|  example/example.js          |a complete example of how to set up and run a JavaScript APG parser|
|  example/example.html        |a simple web page for implementing the example parser|
|  example/iniFileOpcodes.js   |the APG-generated opcodes object for the example grammar|
|  example/iniFile.bnf         |the example ABNF grammar used to generate the parser&acute;s opcodes object|
|  LICENSE                     |Version 2 of the GNU General Public License|
|  README.md                   |this file|

**Documentation:**  
To generate the documentation install <a href="https://github.com/jsdoc3/jsdoc">jsdoc</a> and from the project directory run:  
`/path/to/jsdoc . README.md -r -d documentation`  
To view the documentation open the file  
`documentation/index.html`  
in any web browser, or view it at the <a href="http://www.coasttocoastresearch.com/">APG website</a>.

**Example:**  
To run the example, open  
`example/example.html` 
in any web browser.

**Copyright:**  
  *Copyright &copy; 2009 Lowell D. Thomas, all rights reserved*  

**License:**  
  JavaScript APG and this Runtime Library, Version 1.0 are released under Version 2.0 or higher of the
  <a href="https://www.gnu.org/licenses/licenses.html">GNU General Public License</a>.

      
