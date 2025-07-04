<show-structure depth="2"/>

# Create competency framework

It is important to have a well-structured competency framework.

You can either create it manually, or import competencies via JSON.

There are three components in a framework: proficiency levels, competency categories, and competencies themselves.

### Proficiency levels

Proficiency levels define the level of expertise in a particular skill.

<procedure title="Add proficiency levels">
    <step>Go to <control>Competency Center > Proficiency levels</control>.</step>
    <step>Click <control>Add level</control>.</step>
    <step>In the dialog, fill in the following options:
    <deflist type="narrow">
        <def title="Level name">
        The name of the proficiency level, like "Expert", "Beginner", or other.
        </def>
        <def title="Description">
        Optionally, describe what this level implies in your organization, for example, the criteria for this level of seniority.
        </def>
    </deflist>
    </step>
    <step>Click <control>Confirm</control> to add the level to the framework. Repeat the process to add more levels.</step>
    <step>After adding sufficient proficiency levels, arrange them in the correct order using the <icon src="Drag.svg"/> <control>Drag</control> handle.</step>
</procedure>

<tip>To edit a proficiency level later, find it in the list and click <icon src="Edit.svg"/> <control>Edit</control> in the proficiency level list. </tip>

### Competency categories

Categories allow you to organize your competency framework into neat sections and subsections.
This approach will make the framework easy to navigate and browse both for learners and managers.

You can also hide certain categories from selected user groups, if they are irrelevant to them.

<tip>
It is a good idea to create categories first before creating competencies,
so that you can immediately specify a parent category for them.
</tip>

<procedure title="Add competency category" id="add-category">
    <step>Go to <ui-path>Competency Center > Competencies</ui-path>.</step>
    <step>Click <control>+ Add category</control>.</step>
    <step>Fill out the fields in the dialog:
        <deflist type="narrow">
            <def title="Category name">
            The name of the category, for example, "Soft skills".
            </def>
            <def title="Description">
            The description of the category. 
            </def>
            <def title="Visibility">
            Define whether the category is visible to all signed-in users or only to chosen user groups.
            </def>
        </deflist>
    </step>
    <step>Click <control>Add</control> to save and create the category.</step>
</procedure>

<note>To edit a category later, find it in the list and click <icon src="MoreActions.svg"/><control>Actions</control> > <control>Edit category</control>. </note>

You can add a subcategory to any category using the same procedure.

<procedure title="Add subcategory">
    <step>Go to <ui-path>Competency Center > Competencies</ui-path>.</step>
    <step>Find the parent category and click <control>+ Add subcategory</control>. </step>
    <step>Follow the <a href="#competency-categories">same steps</a> as when creating a parent group.</step>
</procedure>

You can hide categories from certain user groups, if needed, since not all competencies are relevant to all users.
<procedure title="Set category visibility" id="hide_category">
    <step>Go to <ui-path>Competency Center > Competencies</ui-path>.</step>
    <step>Find the category in the list and click <icon src="MoreActions.svg"/><control>Actions</control> > <control>Edit category</control>.</step>
    <step>In the <control>Visibility</control> setting, define who can see the category:
        <deflist type="narrow">
        <def title="All users">All users can see the category. Enabled by default.</def>
        <def title="Select user groups">Select the user groups who will be able to see the category.</def>
        </deflist>
    </step>
<step>Save your category.</step>
</procedure>

### Competencies

A competency describes a specific skill or work knowledge.  

<note>You can also import competencies in bulk via <a href="Import-competencies.md">JSON</a> files.</note> 

<procedure title="Add competencies">
<step>Go to <ui-path>Competency Center > Competencies</ui-path>.</step>
<step>Click <control>+ Add competency</control>. 
    <tip>If you open an existing competency category first, you can immediately add a new competency to it
    by clicking <control>+ Add competency</control> <emphasis>inside</emphasis> that group. </tip>
</step>
<step>Fill in the details:
<deflist type="narrow">
<def title="Name">
The name of the competency, for example, "Team leadership".
</def>
<def title="Description">
Describe the competency. For example, "Team leadership involves guiding and motivating a group to achieve common goals."
</def>
<def title="Parent category">
If you have existing categories, you can define which one is the parent group for this competency. Otherwise, it will be put on a root level.
<warning>We strongly recommend using <a href="#add-category" summary="">categories</a> to organize your competency framework. Uncategorized competencies are sorted alphabetically.</warning>
</def>
</deflist>
</step>
<step>Click <control>Confirm</control> to add the competency. </step>
</procedure>
<note>To edit a competency, find it in the list and click <icon src="MoreActions.svg"/><control>Actions</control> > <control>Edit competency</control>. </note>

