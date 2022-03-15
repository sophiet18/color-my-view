# udacity-3
So I almost had a heart attack when I realized acitvity main tags weren't showing up again... 

This time I learnt about constraints, chains, and ratios 
AND IMPORTANT REMINDER TO ALWAYS CHECK TO SEE IF THE ANDROID PLUGIN IS ADDED

📍CONSTRAINT 
a connection or alignment to another UI element, to the parent layout or to an invisible guideline 

🌟 ADVANTAGES 
• can be made responsive to screens and resolutions
• usually flatter view hierarchy
• optimized for laying out its views
• FREE FORM - views can be placed anywhere and the editor helps you add constraints 

📌 FIXED CONSTRAINTS
• represented by a straight line 
• a common use is for margins 

📌 WRAP CONTENT
• represented by a line of chevrons 
• the view expands only as much as needed  to fit its contents 

📌 MATCH CONSTRAINTS (0dp)
• represented by the zigzag line 
• the more constraints of this kind, the roe the layout can adapt to different screen sizes and orientations = fewer layouts for the app
• ⚠️ this is coded as 0dp!!  

IFFFF there are many views with many constraints, the Android system will work out how to meet all those constraints to create a layout 

📌 FIXED CONSTRAINT
• a constraint that is specified with a hardcoded number

📌 ABSOLUTE POSITION
• specified with layout_margin
• position is NUMERICAL
• IF you don't specify a position for a view, the default is 0,0 (X,Y coordinates) in the parent at the top left corner

📌 RELATIVE POSITIONING
• specifies where the view goes in relation to other views, INCLUDING the parent
• views are positioned by specifying relationship to other views 

📌 ADAPTABLE CONSTRAINTS
• a more powerful constraint
• specifies a relationship between views, and the system figures out where the view ends up
• adding a flexible constraint to each edge of the parent centers the view because it is connected equally to both edges  
• a constraint that defines a relationship in relative and weighted terms 

📌 BIAS
• adding bias gives a preference or more weights to a constraint, like adding a stronger spring to one side of the view

⚠️ORDER MATTES
• when connecting baseline from of multiple items, the items cannot duplicate in being the beginning and the end
• from each handle there can only be one constraint!
• example: when connecting ABC, A -> B and then C->B 

CHAINS
links views in horizontal or vertical rows together so that they behave as a group 

different views are considered linked/chained together if they're connected together via a BIDIRECTIONAL connection 

chains are controlled by attributes set on the head of the chain and alignment is controlled by assigning weight and bias to elements

HEAD = the element at which the chain was created 

📌 SPREAD CHAIN
• aka the default behaviour of chains, views are spread equally within the available space 

📌 SPREAD INSIDE CHAIN
• uses all available space BETWEEN head and tail elements of a group 

📌 WEIGHTED CHAIN
• uses up all space and resize elements to fit it, based on the values set in the layout constraint horizontal weight or layout constraint vertical weight attributes 

📌 PACKED CHAIN [ with bias] 
• uses minimum space
• can add bias to move the group of elements on the axis

RATIO
Ratios are most useful when your layout has views that need to keep their shape/aspect ratio even when the screen orientation or dimensions change.

creating a SQUARE... as an example 
• made with a 1:1 ratio 
• especially useful for adaptive layouts, so that you don't have to hardcode each dimension for different devices 
• can also be edited in the layout editor

📌A view needs to have a certain aspect ratio to accommodate an image, no matter what the screen orientation or display size is 

📌You want to create a layout with squares that is adaptable but forces the square to remain square 

