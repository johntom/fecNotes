         f965ab2fe692ef7a7ae23e20303e26319e57e043 access tolken
     xxx    
================= April 27 ====================
x add offerings
x1) as detail to Inventory
inventory#,client, the amount, date
x2) as option in actions
Actions fix search on nothing

3) Must enter Exhibition so you can select on the Reproduction tab when
making a catalog entry () the title and type=Catalog of Repro should be populated by the dropdown
reorder cols to select exhibit , title
Look at exhibit tab Reproduction column for logic to get dropdown

4) Open (download) doc file from fs
DELANE0215
LEWIS00114
HOFMAN0015
================= April 27 End====================

         
            matt raise horizontal tabs see css flex section 
            matt wont save searhc box info
            matt async await
            matt new components Must be amd compatible
            matt http
            x Change message moving off form check for dirty
            x Give message of success save. Auto close form
            hilite detail tab after selection
            fix drops on detail tabs
            
            FS fix

           x PURCHASED Turns to green

            x add button on search for inventory
           
            consiged to

I would use blue for the “+ add” button on the tabs
(it is currently a mix of blue & green)

Should the tab that is currently displayed turn blue so it is easy to identify?

I think the heading font on each of the tabs is too large, we might discuss what this should look like

Switching between Cosignedto/Museumloan/Insurance/Vat/Purchased/Consigned- can take a really long time, the rest of the tabs respond quickly

Notes Tab
   x 1.    “+ add” button is green
   x 2.    Inventory Title not inc in heading

Exhibition Tab
    x 1.    “+ add” button is blue
    2.    “traveled” y/n field

Provenance Tab
  x  1.    “+ add” button is blue
  y  2.    “+ add” not working

Reproduction Tab
  x  1.    “+ add” button is blue
  x  2.    Blue background for column labels extends down into the fields (on the Provenance and Exhibition tabs it is grey)
    3.    Fields to link up:
        “Repro Type”  (typo on label)
        “ColorBW”
        “Repro SortDate” (text field)
        “Set Exhibition”

Transport Tab
 x   1.    Inventory Title not inc in heading, says “Transport v5”
 x   2.    “+ add” not working
 x   3.    “+ add” button is green
 ? show a date for me   4.    do we want a calendar control on “TransportDate”?

Docs Tab
    1.    Inventory Title not inc in heading but Inventory Code is
    2.    “+ add” button is green

Consignedto Tab
 x   1.    Inventory Title not inc in heading, says “v102 for 1”
 x   2.    “+ add” button is green
 x   3.    “+ add” not working
    4.    “retail price” is there twice  YES coded
    5.    Which of the price fields should look up to the alpha code and which should look up to the actual price?
    6.    “to” field not hooked up


Conservation Tab
   x 1.    header says “Notes”
   x 2.    “+ add” button is green
  x  3.    “+ add” not working
  x  4.    Inventory Title not inc in heading
    5.    can not edit existing data
    6.    clicking update brings up live fields in a strange places:
        If you enter data in any of the live fields, it fills all the fields except “ConcervedBy”
        “ConservedBy” gets replaced by a date field
        When you enter data in the live field that appears under “Treatment” it wants to auto fill with email address data that is stored on my machine locally
        the live fields that appear under “Dates” & “Invoice No” don’t have that behavior

Museumloan Tab
    1.    header says “Museam”
    2.    “+ add” button is blue
    3.    “+ add” not working
    4.    what type of field is “Artwork”,  is it really a date?

photo Tab
 x   1.    Inventory Title not inc in heading and it says “Museam”
 x   2.    “+ add” button is blue
 x   3.    can’t test; add photo doesn’t do anything

image track Tab ?

condition Tab

  x 1.    Inventory Title not inc in heading
  x  2.    “+ add” button is green
  x  3.    “+ add” not working, so can’t test


rtf Tab: not using

Purchased Tab
    1.    “Date”: should this be a calendar control?

Consigned- Tab
    1.    what is this?
    2.    is “Shipping ID” really supposed to look up to a list of names?
    3.    is “signed” a text field or y/n?
    4.    does net price display the alpha code or the actual price?

Insurance/VAT
    1.    layout is a little uneven
    2.    “TaxAmtPaid” is there twice
    3.    Which of the currency fields  (InsuredAmt/TaxAmtPaid/TaxPrepaid) point to the alpha code and which display actual price
    4.    Should “ReimburseDate” and “ReimburseDateRequested” be calendar controls?

Editions Tab

Soldto Tab
    1.    Should “SoldDate” be a calendar control?
    2.    do “SoldPayment” & “SoldPrice” point to alpha code or display actual price?




==================================================mas====================================
mas - closed cycle for part time adjuster payments
mas - no rule for Invoice
mas - type a head for table entries
mas - generate next avail inv #
mas - chk data for 01-03188 fix contacts

						01-03188
			x	move footer
				
			x	move tabs
				
			x	see extend description
				
			x	format table
				
			x	fix formfooter
				
				Do Uploader
				
			x	local image vs http://adjusters.markadjustment.com/docs/images/MAimage.jpg
				
        
						object sizes for BS fixed with css
					</li>
        
        -->