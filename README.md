# validate-testNG-xml
Validate TestNg XML and update it to your needs

* The TestNgXMLUpdater program implements an logic that does the below operations:
 * 1. Remove test-method nodes where status = "Skip"
 * 2. Remove test-method nodes where the name does not end in "Test". This removes things like beforeClass, afterClass, etc.
 * 3. In each test-method node, append a unique number [1],[2],[3], etc. to each name attribute. This forces ALM to bring these in a separate tests, otherwise ALM will bring these in as different runs for the same test
