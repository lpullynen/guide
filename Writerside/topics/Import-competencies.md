# Import competencies

<!--suppress WrsCodeBlockWidthInspection -->
<show-structure depth="2"/>

You can import the competencies, categories, and proficiency levels from a JSON file into Competence Center instead of manually creating them.

If you already have some data in place, the import will only update the data that matches the items in the imported file. It will not delete the rest.

<note>You can download a <resource src="import_sample.json">sample JSON file</resource> to serve as a basis.
It includes some examples of levels, competencies, and categories.</note>


<warning>The imported file size should not exceed 5 MB.</warning>

## JSON file structure 

Here's the content structure of the sample file.

[//]: # (Content referenced from a file)
<code-block lang="JSON" collapsible="true" show-white-spaces="true" collapsed-title="import_sample.json" src="import_sample.json"/>

### Root level
The root level includes the proficiency levels and categories to be imported.
<table>
  <tr>
    <th>Section</th>
    <th>Field</th>
    <th>Type</th>
    <th>Required</th>
    <th>Description</th>
  </tr>

  <!-- Proficiency Levels -->
  <tr><td rowspan="3"><strong>proficiencyLevels</strong></td><td><code>id</code></td><td>string</td><td>Yes</td><td>Unique identifier for the proficiency level</td></tr>
  <tr><td><code>name</code></td><td>string</td><td>Yes</td><td>Display name shown in the UI</td></tr>
  <tr><td><code>description</code></td><td>string</td><td>No</td><td>Description of the level</td></tr>

  <!-- Competency Categories -->
  <tr><td rowspan="4"><strong>competencyCategories</strong></td><td><code>id</code></td><td>string</td><td>Yes</td><td>Unique identifier for the category</td></tr>
  <tr><td><code>name</code></td><td>string</td><td>Yes</td><td>Display name of the category</td></tr>
  <tr><td><code>description</code></td><td>string</td><td>No</td><td>Description of what the category covers</td></tr>
  <tr><td><code>competencies</code></td><td>array</td><td>Yes</td><td>Array of competency objects in this category</td></tr>
</table>

### Competencies
Competencies in the import file are nested inside <code>competencyCategories</code>.
<table>
 <tr>
    <th>Section</th>
    <th>Field</th>
    <th>Type</th>
    <th>Required</th>
    <th>Description</th>
  </tr>
  <!-- Competencies -->
  <tr><td rowspan="3"><strong>competencies</strong></td><td><code>id</code></td><td>string</td><td>Yes</td><td>Unique identifier for the competency</td></tr>
  <tr><td><code>name</code></td><td>string</td><td>Yes</td><td>Display name of the competency</td></tr>
  <tr><td><code>description</code></td><td>string</td><td>No</td><td>Description of what the competency involves</td></tr>
</table>

<procedure title="Import competencies">
<step>Go to <ui-path>Competency Center > Competencies</ui-path>.</step>
<step>In the <icon src="MoreActions.svg" alt="Actions"/><control>Actions</control> menu, 
click <control>Import competencies (JSON)</control>.
</step>
<step>Drag and drop your file or browse yor computer.</step>
<step>Click <control>Upload competencies</control>. The file contents will be validated upon upload. If the validation is successful, the data will be imported.
<tip>If validation fails, you will get more information in the error messages.</tip></step>
</procedure>