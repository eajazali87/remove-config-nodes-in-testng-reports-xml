# modify-testng-reports.xml
Modify testNg-reports.xml and update it to your needs. For eg, add, remove or update a node.

* The TestNgXMLUpdater program implements an logic that does the below operations:
 * Remove &lt;test-method&gt; nodes where status = "Skip"
 * Remove &lt;test-method&gt; nodes where the name does not end in "Test". This removes things like beforeClass, afterClass, etc.
 * In each &lt;test-method&gt; node, append a unique number [1],[2],[3], etc. to each name attribute. This forces ALM to bring these in a separate tests, otherwise ALM will bring these in as different runs for the same test
 
#####NOTE: You could pass a specific node and modify the IF condition according to your requirement.
