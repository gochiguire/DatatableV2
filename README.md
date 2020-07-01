# DatatableV2

Lightning Web Component for Flow Screens:       **datatableV2**

**This component allows the user to configure and display a datatable in a Flow screen.**

Additional components packaged with this LWC:

                    Lightning Web Components:   datatableV2Spring20 (temporary version for hardcoded SObjects)   

                    Apex Classes:               SObjectController2 
                                                SObjectController2Test  
                                                  
**Documentation:**  https://unofficialsf.com/datatablev2-lightning-web-component-for-flow-screens/  
  
**Created by:**	Eric Smith  
**Date:**		March 2020
  
LinkedIn: https://www.linkedin.com/in/ericrsmith2  
Salesforce: https://trailblazer.me/id/ericsmith  
Blog: https://ericsplayground.wordpress.com/blog/  
Twitter: https://twitter.com/esmith35  

---

<a href="https://githubsfdeploy.herokuapp.com">
  <img alt="Deploy to Salesforce"
       src="https://raw.githubusercontent.com/afawcett/githubsfdeploy/master/deploy.png">
</a>

---

## Release Notes
07/01/20 -  Eric Smith -    Version 2.36 -  
            Updates:        Now displays the primary "Name" field as a Link (textWrap = true)
              
06/30/20 -  Eric Smith -    Version 2.35 -  
            Updates:        Extended Configuration Mode to handle Column Alignments, Labels, Widths, Allow Edit & Allow Filter  
                            Added Configuration Mode buttons to select all columns for Edit and/or Filter  
                            Selecting an attribute string now copies the contents into the system Clipboard  
                              
06/24/20 -  Eric Smith -    Version 2.34 -  
            Updates:        Added Configuration Mode parameter (Used by Datatable Configuration Flow)  
            Bug Fix:        Fixed issue with column widths resetting when filtering  
  
06/19/20 -  Eric Smith -    Version 2.33 -  
            Updates:        Removed default value for Table Height
            Bug Fix:        Fixed issue with lookup fields being blank in the first record                                                    
  
06/03/20 -  Eric Smith -    Version 2.32 -  
            Bug Fix:        Fixed error when editing more than one column in a single row while suppressing the Cancel/Save buttons
  
06/03/20 -  Eric Smith -    Version 2.31 -  
            Updates:        Changed SObjectController to SObjectController2 to allow for easier deployment to orgs 
                            that already have an earlier version of the datatable component    
                                                                                   
06/03/20 -  Eric Smith -    Version 2.3 -  
            Updates:        Changed SObjectController to SObjectController2 to allow for easier deployment to orgs 
                            that already have an earlier version of the datatable component
  
06/03/20 -  Eric Smith -    Version 2.2 -  
            Enhancements:   Added datatable border attribute
            Updates:        Fixed attribute parsing, Fixed Spinner
  
06/01/20 -  Eric Smith -    Version 2.1 -  
            Enhancements:   Updated with features from v1.2 & v1.3                                                
  
04/22/20 -  Eric Smith -    Version 2.0 (Summer '20) -  
            Enhancements:   Summer '20 New Feature - Dynamic Object Type
                            One version of the component now supports ALL Standard & Custom SObjects
  
05/23/20 -  Eric Smith -    Version 1.3 -  
            Updates:        Added support for a serialized JSON string of records of a user defined object
                            Added an attribute to specify the height of the datatable
                            Bug Fix - Fixed error when editing multiple rows           
  
05/06/20 -  Eric Smith -    Version 1.2 -  
            Updates:        Handle lookup Objects without a Name field & 
                            Trap non-updatable Master/Detail fields
  
04/14/20 -  Eric Smith -    Version 1.1 -  
            Enhancements:   New Column Attribute to support column filtering  
  
04/01/20 -  Eric Smith -    Version 1.0 -  
Features:   The only required paramters are the SObject collection of records and a list of field API names  
            The field label and field type will default to what is defined in the object  
            Numeric fields will display with the correct number of decimal places as defined in the object  
            Lookup fields are supported and will display the referenced record's name field as a clickable link  
            All columns are sortable, including lookups (by name)  
            The selection column can be multi-select (Checkboxes), single-select (Radio Buttons), or hidden  
            A collection of pre-selected rows can be passed into the component  
            Inline editing is supported with changed values passed back to the flow  
            Unlike the original datatable component, only the edited records will be passed back to the flow  
            The maximum number of rows to display can be set by the user  
            Optional attribute overrides are supported and can be specified by list, column # or by field name, including:  

                - Alignment               
                - Editable
                - Header Icon
                - Header Label
                - Initial Column Width
                - Custom Cell Attributes including those with nested values {name: {name:value}}               
                - Custom Type Attributes including those with nested values {name: {name:value}}
                - Other Custom Column Attributes including those with nested values {name: {name:value}}
  
---

Copyright (c) 2020, Eric Smith

Redistribution and use in source and binary forms, with or without modification, are permitted provided 
that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer 
in the documentation and/or other materials provided with the distribution.

3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived 
from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, 
BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT 
SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL 
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS 
INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING 
NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.