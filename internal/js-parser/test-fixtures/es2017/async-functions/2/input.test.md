# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `es2017 > async-functions > 2`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: false
	directives: Array []
	filename: "es2017/async-functions/2/input.js"
	hasHoistedVars: false
	interpreter: undefined
	mtime: undefined
	sourceType: "script"
	syntax: Array []
	loc: Object {
		filename: "es2017/async-functions/2/input.js"
		end: Object {
			column: 0
			line: 4
		}
		start: Object {
			column: 0
			line: 1
		}
	}
	diagnostics: Array [
		Object {
			origins: Array [Object {category: "parse/js"}]
			description: Object {
				advice: Array []
				category: "parse/js"
				message: MARKUP {parts: Array [RAW_MARKUP {value: "await* has been removed from the async functions proposal. Use Promise.all() instead."}]}
			}
			location: Object {
				filename: "es2017/async-functions/2/input.js"
				mtime: undefined
				sourceText: undefined
				end: Object {
					column: 2
					line: 2
				}
				start: Object {
					column: 2
					line: 2
				}
			}
		}
	]
	body: Array [
		JSFunctionDeclaration {
			id: JSBindingIdentifier {
				name: "bar"
				loc: Object {
					filename: "es2017/async-functions/2/input.js"
					identifierName: "bar"
					end: Object {
						column: 18
						line: 1
					}
					start: Object {
						column: 15
						line: 1
					}
				}
			}
			loc: Object {
				filename: "es2017/async-functions/2/input.js"
				end: Object {
					column: 1
					line: 3
				}
				start: Object {
					column: 0
					line: 1
				}
			}
			head: JSFunctionHead {
				async: true
				generator: false
				hasHoistedVars: false
				params: Array []
				rest: undefined
				returnType: undefined
				thisType: undefined
				typeParameters: undefined
				loc: Object {
					filename: "es2017/async-functions/2/input.js"
					end: Object {
						column: 20
						line: 1
					}
					start: Object {
						column: 18
						line: 1
					}
				}
			}
			body: JSBlockStatement {
				directives: Array []
				loc: Object {
					filename: "es2017/async-functions/2/input.js"
					end: Object {
						column: 1
						line: 3
					}
					start: Object {
						column: 21
						line: 1
					}
				}
				body: Array [
					JSExpressionStatement {
						loc: Object {
							filename: "es2017/async-functions/2/input.js"
							end: Object {
								column: 15
								line: 2
							}
							start: Object {
								column: 2
								line: 2
							}
						}
						expression: JSAwaitExpression {
							loc: Object {
								filename: "es2017/async-functions/2/input.js"
								end: Object {
									column: 14
									line: 2
								}
								start: Object {
									column: 2
									line: 2
								}
							}
							argument: JSCallExpression {
								arguments: Array []
								loc: Object {
									filename: "es2017/async-functions/2/input.js"
									end: Object {
										column: 14
										line: 2
									}
									start: Object {
										column: 9
										line: 2
									}
								}
								callee: JSReferenceIdentifier {
									name: "foo"
									loc: Object {
										filename: "es2017/async-functions/2/input.js"
										identifierName: "foo"
										end: Object {
											column: 12
											line: 2
										}
										start: Object {
											column: 9
											line: 2
										}
									}
								}
							}
						}
					}
				]
			}
		}
	]
}
```

### `diagnostics`

```

 es2017/async-functions/2/input.js:2:2 parse/js ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ await* has been removed from the async functions proposal. Use Promise.all() instead.

    1 │ async function bar() {
  > 2 │   await* foo();
      │   ^
    3 │ }

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```
