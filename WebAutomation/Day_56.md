## Learning Goal
Test report generation

### Problem Statement
You need to add a report generator component to your web automation framework which will allow users to select any reporting framework from configuration provided.

### Detail steps to be automated
- Open https://www.makemytrip.com/ web site.
- Verify that Make My Trip title is displayed.

### Configuration options
Report_Framework_Name = supported values - Default or Extend_Report or Allure_Report

Note: Detault report means the report generates by the unit test framework used. For example TestNG default report.

### Hints
- Use oops concepts to build the reporting module.
- Your reporting module should be open for adding any new reporting framework without impacting the existing test cases or any other modules of your framework.
