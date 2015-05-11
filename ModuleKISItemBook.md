#### `ModuleKISItemBook`

Allow an item to be used like a book.

Sample module configuration :
```
MODULE
{
	name = ModuleKISItemBook
	pageWidth = 800
	pageHeight = 800
	bookOpenSndPath = KIS/Sounds/bookOpen
	bookPageSndPath = KIS/Sounds/bookPage
	bookCloseSndPath = KIS/Sounds/bookClose
	page = KIS/Parts/guide/page01
	page = KIS/Parts/guide/page02
}
```

- `pageWidth`: Width of all pages.
- `pageHeight`: Height of all pages.
- `bookOpenSndPath`: Change opening book sound.
- `bookPageSndPath`: Change previous/next page sound.
- `bookCloseSndPath`: Change closing book sound.
- `page`: Path of the page image. Can be repeated. Pages will be sorted in the stated order.
