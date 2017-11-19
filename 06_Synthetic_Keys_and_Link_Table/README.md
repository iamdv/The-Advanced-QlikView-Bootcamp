This chapter shows advanced techniques to create link tables and ways to handle synthetic key

ink:
LOAD
	*,
	date(subField(%LinkKey, '|', 1), 'M/D/YYYY')	AS  Date,			 
	subField(%LinkKey, '|', 2)						AS  [Product ID]	     
;
LOAD
	FieldValue('%LinkKey', RecNo()) 				AS %LinkKey
AUTOGENERATE FieldValueCount('%LinkKey')
;


DROP FIELDS [Order Date], [Purchase Date], [Inventory Date], [Product ID], %SalesLinkKey FROM Sales, Purchases, Inventory;  

