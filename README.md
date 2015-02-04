# DateRangeHTML5WebControl
A sample HTML5 web control implementation of a date range control.

The date range control is implemented in the file tt-daterange-template.html. 

To use the custom element,

1. Import the html template file   
`<link rel="import" href="tt-daterange-template.html" />`
2. Declare the date range element in the markup     
`<tt-date-range id="dtEmp1">`
3. The control provides two content placeholders - selected by the class labelFrom and labelTo. If declared, these will get distributed into the shadow tree content elements.

           <tt-date-range id="dtEmp1">
              <span class="labelFrom">From #1</span>
              <span class="labelTo">To #1</span>
           </tt-date-range>
4. To get the date values, get the reference to the custom element and call the getDateValueFrom and getDateValueTo functions.
  
          dtEmp = document.querySelector("#dtEmp1");
          date1 = dtEmp.getDateValueFrom();
          date2 = dtEmp.getDateValueTo();

This is just a sample project using native HTML5 Web components, at the time it is only suported in Chrome.
