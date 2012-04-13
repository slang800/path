#PATH (pre-alpha)
##Description
PATH is (P)HP (A)rrays (T)o (H)TML, which allows you to express HTML code as arrays written in a JSON-based shorthand, and converts these arrays into regular HTML.

 - easier to manipulate and search through than regular text
 - written less redundantly than HTML (no end tags)
 - automatically determine things like self-closing tags
 - language-agnostic: by exporting into JSON, you can write PATH in any language or even store PATH in a db like mongo
 - whitespace agnostic (format your PATH however you please)
 - compiled HTML can be compressed (whitespace removed) or indented like regular HTML

For example:

	<label id="myId" style="background:#000">this is my content</label>
can be written as

	['label#myId','style'=>'background:#000','this is my content']
or

	['label#myId',
		'style'=>'background:#000',
		'this is my content'
	]
(whichever you like)

##Features
 - id & class shorthands - rather than specifying an id or classes as attributes, they can be combined with the tag name in a format resembling a CSS seclector
	
 - default div tag - if no tag is specified, a div tag will be assumed
	



PATH is not a new way to write HTML, it is a new way to write templates which is more closely intergrated with PHP. If you use PATH just for writing static HTML, and you are not using functions or shorthand to automate the writing of your pages, then you are wasting your time. 