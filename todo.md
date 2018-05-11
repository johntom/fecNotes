         f965ab2fe692ef7a7ae23e20303e26319e57e043 access tolken
     xxx 
================= May 11 ====================

**General Issues**
1. need to be systematic and judicious about when we use pop up to tell you to save or that you have saved
 * if i have 2 inventory items opened from a search and i am switching between them to figure out which is the one i want to edit, I get a message asking me if I want to leave the form without saving even thought I haven't changed anything
 * if I click "stay & save" I then have to click ok in the pop up that tells me that I have saved
 * I believe there have been times where I changed something on a tab form and then was able to switch to another tab without saving and without getting a warning
2. When we use a pop up to fill in a look up field instead of a dropdown we have to follow the rules of Capitalization & spaces between words that they are so nutty about 
3. I think the header font is a little big on these pop up forms

**inventory form: header fields**
1. remove MRG Location field
2. are keywords adding on the fly?
3. think from Hoopers notes we need all 4 dimension fields
 * Size (no need to say “unframed”)
 * Sight size
 * Framed size
 * Image size

**General Tab Issues**
1. when on a 1:many tab form, if I click the "Update" button to edit a record, the whole page tries to reload and it gets stuck
2. These are (I think) all the tabs that use the pop up forms which need to have the formatting/wording changed. 
 * Conserved By
 * Sold To
 * Purchased From
 * Loan To
 * Consigned To
 * Consigned From  (there are 2 pop ups on this tab)

3. These are the things that have to be checked
 * name of form: make sure the name corresponds to the form and that it has a space between words: Consigned To not Consignedto
 * the text where it says "type any characters of the Purchased From (not PurchasedFrom) to select
 * make sure the words in the box that you are typing into correspond to the correct field (see Purchased From & loan To)


**Prov Tab**
add+ button gives a message when you click it, I believe it's the only one


**Exhibition Tab**
I think there is still an extra field here (from when you were considering choosing a reproduction to associate)
so the column headings are off

**Conservation Tab**
1. Still has (title ct:) in the header of the tab
2. Labels that need correction: label ConservedBy, InvoiceNo and Cmd

**Sold To Tab**
Check dropdown for Payment Method

**Purchased From Tab**
1. still has the word "Purchased" needs to conform to Sold To tab 
2. correct PaymentNo and Notes

**Loan To  Tab**
1. Ins Value,  Ins Amt,  MRG Signed, Institution Signed, Note, Updated Fact Sheet
2. We have to check on these fields: cofl? Artwork field date? 

**Consigned To**
1. check column labels
2. not sure if they need them but are created and modified dates being generated?

**Consigned From Tab**
Labels: Notes, netPrice

**Editions Tab**
publisher and printer locations not saving

================= May 11 End ====================

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