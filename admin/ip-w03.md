{% from "common/macros.njk" import thumb with context %}
{% macro show_main_text() %}
<div id="main">

<div id="title">

</div>
<div id="body">

In this week, we try to practice git branching as we do the iP.

{{ thumb(1) }} Do Level 7 in a branch named `branch-level7`. Without merging that branch, go back to the `master` branch and implement Level 8 in a separate branch named `branch-level8`. Now, go back to the `master` branch and merge the two branches one after the other. As before, tag the commit (in the `master` branch, after merging) that achieves the respective deliverable, and push to your fork.

<include src="dukeFragment.md" boilerplate var-header="**`Level-7`: Save**" var-fragment="text.md#level7" />
<include src="dukeFragment.md" boilerplate var-header="**`Level-8`: Dates and Times**" var-fragment="text.md#level8" />

<p/>

{{ thumb(2) }} As in the previous week, commit, tag, and push, as you do the following increments in the `master` branch (no need to use separate branches).
<include src="dukeFragment.md" boilerplate var-header="**`A-MoreOOP`: More OOP**" var-fragment="extensions.mbdf#A-MoreOOP" />
<include src="dukeFragment.md" boilerplate var-header="**`A-Packages`: Java Packages**" var-tag="optional" var-fragment="extensions.mbdf#A-Packages" />
<include src="dukeFragment.md" boilerplate var-header="**`A-JUnit`: JUnit Testing**" var-fragment="extensions.mbdf#A-JUnit" />
<include src="dukeFragment.md" boilerplate var-header="**`A-Jar`: JAR file**" var-fragment="extensions.mbdf#A-Jar" />

<p/>

{{ thumb(3) }} As in the step 1 above, implement these three increments as three parallel branches first, and then merge them one-by-one. Hopefully, you will encounter some merge conflicts so that you get to practice de-conflicting branches.
<include src="dukeFragment.md" boilerplate var-header="**`A-JavaDoc`: JavaDoc**" var-fragment="extensions.mbdf#A-JavaDoc" />
<include src="dukeFragment.md" boilerplate var-header="**`A-CodingStandard`: Coding Standard**" var-fragment="extensions.mbdf#A-CodingStandard" />
<include src="dukeFragment.md" boilerplate var-header="**`Level-9`: Find**" var-fragment="text.md#level9" />

<p/>

{{ thumb(4) }} Create a pull request (PR) from the `master` branch of your fork to the upstream repo.
* PR name: `[Your name] Duke Increments` e.g., `[John Doe] Duke Increments` %%If you are reluctant to give full name, you may give the first half of your name only%%

<br>
</div>
</div>
{% endmacro %}

{% from "common/admin.njk" import show_admin_page with context %}
{{ show_admin_page("ip-w03", show_main_text) }}