Function.introspect.js is a small library that interrogates a function to return its name, argument names and source code (if not native).

Use it like this:

	function add(a, b) { return a + b; }
	var finfo = Function.introspect(add);
	// finfo => {
	//	name: 'add',
	//	args: 'a,b',
	//	argNames: ['a','b'],
	//	code: 'return a+b;',
	//	isNative: false
	// }

Compatibility: IE 6-8, Firefox 3-3.5, Safari 3-4, Chrome 3, node.js.