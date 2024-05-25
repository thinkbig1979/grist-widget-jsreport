# Grist Custom Widget To Fetch JSReport Report

This widget reads a formula from the "template" column of the selected record.
The record should be formatted as follows:


```javascript
{
      template: {
        url: "https://yourJSreportserver.com",
        user: "username",
        pw: "password",
        body: {
          template: { name: "JSreport Template Name" },
          data: {
            yourData:"value"
          },
        },
      },
    };

``` 

Clicking the button in the widget then fetches and downloads the generated report.
