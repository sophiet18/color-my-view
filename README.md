# lesson 2 part 2
So I almost had a heart attack when I realized acitvity main tags weren't showing up again... 

This time I learnt about constraints, chains, and ratios 
AND IMPORTANT REMINDER TO ALWAYS CHECK TO SEE IF THE ANDROID PLUGIN IS ADDED

πCONSTRAINT 
a connection or alignment to another UI element, to the parent layout or to an invisible guideline 

π ADVANTAGES 
β’ can be made responsive to screens and resolutions
β’ usually flatter view hierarchy
β’ optimized for laying out its views
β’ FREE FORM - views can be placed anywhere and the editor helps you add constraints 

π FIXED CONSTRAINTS
β’ represented by a straight line 
β’ a common use is for margins 

π WRAP CONTENT
β’ represented by a line of chevrons 
β’ the view expands only as much as needed  to fit its contents 

π MATCH CONSTRAINTS (0dp)
β’ represented by the zigzag line 
β’ the more constraints of this kind, the roe the layout can adapt to different screen sizes and orientations = fewer layouts for the app
β’ β οΈ this is coded as 0dp!!  

IFFFF there are many views with many constraints, the Android system will work out how to meet all those constraints to create a layout 

π FIXED CONSTRAINT
β’ a constraint that is specified with a hardcoded number

π ABSOLUTE POSITION
β’ specified with layout_margin
β’ position is NUMERICAL
β’ IF you don't specify a position for a view, the default is 0,0 (X,Y coordinates) in the parent at the top left corner

π RELATIVE POSITIONING
β’ specifies where the view goes in relation to other views, INCLUDING the parent
β’ views are positioned by specifying relationship to other views 

π ADAPTABLE CONSTRAINTS
β’ a more powerful constraint
β’ specifies a relationship between views, and the system figures out where the view ends up
β’ adding a flexible constraint to each edge of the parent centers the view because it is connected equally to both edges  
β’ a constraint that defines a relationship in relative and weighted terms 

π BIAS
β’ adding bias gives a preference or more weights to a constraint, like adding a stronger spring to one side of the view

β οΈORDER MATTES
β’ when connecting baseline from of multiple items, the items cannot duplicate in being the beginning and the end
β’ from each handle there can only be one constraint!
β’ example: when connecting ABC, A -> B and then C->B 

CHAINS
links views in horizontal or vertical rows together so that they behave as a group 

different views are considered linked/chained together if they're connected together via a BIDIRECTIONAL connection 

chains are controlled by attributes set on the head of the chain and alignment is controlled by assigning weight and bias to elements

HEAD = the element at which the chain was created 

π SPREAD CHAIN
β’ aka the default behaviour of chains, views are spread equally within the available space 

π SPREAD INSIDE CHAIN
β’ uses all available space BETWEEN head and tail elements of a group 

π WEIGHTED CHAIN
β’ uses up all space and resize elements to fit it, based on the values set in the layout constraint horizontal weight or layout constraint vertical weight attributes 

π PACKED CHAIN [ with bias] 
β’ uses minimum space
β’ can add bias to move the group of elements on the axis

RATIO
Ratios are most useful when your layout has views that need to keep their shape/aspect ratio even when the screen orientation or dimensions change.

creating a SQUARE... as an example 
β’ made with a 1:1 ratio 
β’ especially useful for adaptive layouts, so that you don't have to hardcode each dimension for different devices 
β’ can also be edited in the layout editor

πA view needs to have a certain aspect ratio to accommodate an image, no matter what the screen orientation or display size is 

πYou want to create a layout with squares that is adaptable but forces the square to remain square 

