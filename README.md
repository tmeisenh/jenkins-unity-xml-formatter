jenkins-unity-xml-formatter
===========================
This is an xsl template that is used to convert the xml test output from
Unity tests to a format Jenkins can read.

This is extremely useful for test driven development in C using
ceedling/unity.

For use in ceedling, edit your project.yml.in file and enable the xml_tests_report plugin.
Now when you run unit tests you will get some xml output in
build/artifacts/test/report.xml.

To get Jenkins working, you'll need the xUnit plugin.  In the dropdown,
select "Custom tool."  The pattern is build/artifacts/test/report.xml.
The custom stylesheet is the unity.xsl found in this repo.

This is not my own work; I found this somewhere on the internet.  I am
simply posting this here on github so that others trying to get Unity C
unit tests running on Jenkins won't have as much hassle as I did.

To the original author: thank you.
